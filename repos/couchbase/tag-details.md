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
$ docker pull couchbase@sha256:9de84627fcb614ffdea20e08bd070e81fb606572bf61df8a316d5677a6619d4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.6` - linux; amd64

```console
$ docker pull couchbase@sha256:84ef86645157a156d758d33832b3a49c1339b1d77702eb3278778917c02bde2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.0 MB (532020334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58ad678e9ec231c108ae4761d227f4d469ff29c0ef7ba5b742fafca6b746df24`
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
# Fri, 13 Oct 2023 07:43:33 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6
# Fri, 13 Oct 2023 07:43:33 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb
# Fri, 13 Oct 2023 07:43:33 GMT
ARG CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa
# Fri, 13 Oct 2023 07:43:33 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 13 Oct 2023 07:43:34 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Fri, 13 Oct 2023 07:43:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 13 Oct 2023 07:43:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 13 Oct 2023 07:44:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 07:44:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 13 Oct 2023 07:44:39 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 13 Oct 2023 07:44:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 13 Oct 2023 07:44:40 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 13 Oct 2023 07:44:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 13 Oct 2023 07:44:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 13 Oct 2023 07:44:41 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 13 Oct 2023 07:44:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 Oct 2023 07:44:41 GMT
CMD ["couchbase-server"]
# Fri, 13 Oct 2023 07:44:41 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 13 Oct 2023 07:44:41 GMT
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
	-	`sha256:99f6de63974d9b749570af50a3746b675e45e5a8a4650f036fdb34d46e18c2b6`  
		Last Modified: Fri, 13 Oct 2023 07:51:25 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00c4a58175bb4f00cd56f289b18fece37016bb4c2a1d645af19e9665ade0592`  
		Last Modified: Fri, 13 Oct 2023 07:52:12 GMT  
		Size: 497.1 MB (497149289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f391182a481ef73a0c0ab3a6024b5a69b7f21b98474db4040a67f661f6421055`  
		Last Modified: Fri, 13 Oct 2023 07:51:25 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e649472c0f465231e1c5718cc5c3a5cbf96b1715fdf7efc7008b33040def055`  
		Last Modified: Fri, 13 Oct 2023 07:51:23 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f56fe0b9735a33cf3be6fc48a578d90f03a69715a28c066e4be7e78fc1d16f4`  
		Last Modified: Fri, 13 Oct 2023 07:51:23 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820aec2c4f3736feee2c2c0dc7e84d72efed62e50f3e9cf8e1eb826e12e6d6ad`  
		Last Modified: Fri, 13 Oct 2023 07:51:23 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e1af6b7af088fedb4895f19c17168df7af26bfd525a38e08ebe0b4667ce89e`  
		Last Modified: Fri, 13 Oct 2023 07:51:23 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0213a0b01f3c015fec705d9c2c220710d158d3111b8bf28d1bba01b0f775d01b`  
		Last Modified: Fri, 13 Oct 2023 07:51:23 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.0.5`

```console
$ docker pull couchbase@sha256:5d9823c688107551d0f4153de5e98505d0fb2b3d3bb99b7a619a84d04ba381dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:7.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:2ebdb38bf4f0c3330c205f1966779479e562cf8f51cf803a26cc352a5cfddcfc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **616.7 MB (616700956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e1d1e932031b1b0c647cd28688b4afd7e9dcbaba460f0e9ed3add403e5ccee9`
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
# Fri, 13 Oct 2023 07:40:46 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5
# Fri, 13 Oct 2023 07:40:46 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb
# Fri, 13 Oct 2023 07:40:46 GMT
ARG CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea
# Fri, 13 Oct 2023 07:40:46 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 13 Oct 2023 07:40:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 13 Oct 2023 07:40:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 13 Oct 2023 07:42:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 07:42:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 13 Oct 2023 07:42:05 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 13 Oct 2023 07:42:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 13 Oct 2023 07:42:05 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 13 Oct 2023 07:42:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 13 Oct 2023 07:42:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 13 Oct 2023 07:42:06 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 13 Oct 2023 07:42:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 Oct 2023 07:42:06 GMT
CMD ["couchbase-server"]
# Fri, 13 Oct 2023 07:42:07 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 13 Oct 2023 07:42:07 GMT
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
	-	`sha256:17d7d10e9d142fc70e227ceb9b178daa7d79ed36af0d26b176229999a2a2150f`  
		Last Modified: Fri, 13 Oct 2023 07:49:25 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24925c079cdf75fc52f3b3c4109e3dba2f5ed77320285c527cfedbc869814bef`  
		Last Modified: Fri, 13 Oct 2023 07:50:20 GMT  
		Size: 581.8 MB (581829904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51dcd503c527731a115e4b5da8f216756ba95d790c44153fb87f6c2e11c0a48`  
		Last Modified: Fri, 13 Oct 2023 07:49:25 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6686a51b4d13ae5b4e3f21385169b8790ce2a83eedca61e7f61a51e527c5e5f`  
		Last Modified: Fri, 13 Oct 2023 07:49:23 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b623a9e24470a10dbd831afc95ff0571b572ccde3bae1061906f25b42cf3867b`  
		Last Modified: Fri, 13 Oct 2023 07:49:23 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0314f2c61a2ca1bd2420f1293e60988fd014cc10ab4851519cb5f433421eae`  
		Last Modified: Fri, 13 Oct 2023 07:49:23 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7c453d64636975972288cc988cffe3f17c944292b1c2e16991de1c6ee18b87`  
		Last Modified: Fri, 13 Oct 2023 07:49:23 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0d7d5fe83e5abaf9456d1635b34f428ab51bb36406817a6509f88d150a6723`  
		Last Modified: Fri, 13 Oct 2023 07:49:23 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.1.6`

```console
$ docker pull couchbase@sha256:8e0421be746581ad8e1c32560c5dad18bcb1dc4129b35ab40126e90d94e9b334
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:7.1.6` - linux; amd64

```console
$ docker pull couchbase@sha256:af6fc4ac2462e4133102e9730fc574cffe857d94ab140b2548d77fc5ecf1ba8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **652.0 MB (652019059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e313655605252ec475e3270221b3d975ac35c9d9ce30934f642e24026141cc`
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
# Fri, 10 Nov 2023 02:31:29 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6
# Fri, 10 Nov 2023 02:31:29 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb
# Fri, 10 Nov 2023 02:31:29 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 10 Nov 2023 02:31:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 10 Nov 2023 02:31:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 10 Nov 2023 02:32:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=d4462e7228c372f761bd83f96fa63a7211544df885c2d2e065202ff663dad6f9            ;;          'amd64')            CB_SHA256=abf410a1f97dd14171cd260d4abb853be003db5ec0a44c8324c846068eb90ce7            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 10 Nov 2023 02:32:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 10 Nov 2023 02:32:57 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 10 Nov 2023 02:32:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 10 Nov 2023 02:32:57 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 10 Nov 2023 02:32:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 10 Nov 2023 02:32:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 10 Nov 2023 02:32:59 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 10 Nov 2023 02:32:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Nov 2023 02:32:59 GMT
CMD ["couchbase-server"]
# Fri, 10 Nov 2023 02:32:59 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 10 Nov 2023 02:32:59 GMT
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
	-	`sha256:191174dc2fdae0ccd3b590fde88f3415924e068016cdf948f131cf67739d2628`  
		Last Modified: Fri, 10 Nov 2023 02:34:55 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8872eee949d51c285aeea4e66f04b56279ecd305ba93f9551e368445497d4c36`  
		Last Modified: Fri, 10 Nov 2023 02:35:57 GMT  
		Size: 617.1 MB (617148011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e0a1b755ccc9a7b525bdb0186c60807f93bf4ed5f09dbbc785096109b579bd`  
		Last Modified: Fri, 10 Nov 2023 02:34:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7204d59c585c6547badfc9c91d84d8a0002f4bf842493cdce761cbf11dee64a`  
		Last Modified: Fri, 10 Nov 2023 02:34:53 GMT  
		Size: 746.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab274fa467540d702716aa6838c1c890cb5be73c83023320c99805b278d53c8d`  
		Last Modified: Fri, 10 Nov 2023 02:34:53 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23319a23df40d9ce4ae83364f0ec90b745b0af326da752510c43d1fb22d93c8`  
		Last Modified: Fri, 10 Nov 2023 02:34:53 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef7150892bce389f2c09c0218a3c88ebfabc41aebe6938334085f0380766cd6`  
		Last Modified: Fri, 10 Nov 2023 02:34:53 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71806bdbdb06e7ca1d154faeae1a670d05527fbe56c7455f976b0e445ebfb073`  
		Last Modified: Fri, 10 Nov 2023 02:34:53 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:7.1.6` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:458dff220edcf4672b52fdc4677dc268a4e8175a259f66cc3f0119e9abe00fbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **622.6 MB (622639193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:023645d7f36f8e44a98a6f71839d814535388b15c3a6c2bf3fca3cd298a32f4c`
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
# Fri, 10 Nov 2023 01:44:34 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6
# Fri, 10 Nov 2023 01:44:34 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb
# Fri, 10 Nov 2023 01:44:34 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 10 Nov 2023 01:44:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 10 Nov 2023 01:44:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 10 Nov 2023 01:45:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=d4462e7228c372f761bd83f96fa63a7211544df885c2d2e065202ff663dad6f9            ;;          'amd64')            CB_SHA256=abf410a1f97dd14171cd260d4abb853be003db5ec0a44c8324c846068eb90ce7            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 10 Nov 2023 01:45:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 10 Nov 2023 01:45:44 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 10 Nov 2023 01:45:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 10 Nov 2023 01:45:45 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 10 Nov 2023 01:45:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 10 Nov 2023 01:45:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 10 Nov 2023 01:45:46 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 10 Nov 2023 01:45:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Nov 2023 01:45:46 GMT
CMD ["couchbase-server"]
# Fri, 10 Nov 2023 01:45:46 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 10 Nov 2023 01:45:46 GMT
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
	-	`sha256:4ffda5421b450b5fe26e86864039e1f859621548c5a669a0e07b276fdecebcc4`  
		Last Modified: Fri, 10 Nov 2023 01:47:11 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c02dc935d32efcc9648883ef289c3db68ac3a67d804069d2fd6da95170127aa`  
		Last Modified: Fri, 10 Nov 2023 01:47:50 GMT  
		Size: 589.3 MB (589325444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d59fcdd23df8ac9d0371fb1b7c95b21632a816f14a642ecdad59153b84a83b`  
		Last Modified: Fri, 10 Nov 2023 01:47:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2a5301f374b0a3d811ab6a096485c45de7688a642c383a6fb7f21864840b04`  
		Last Modified: Fri, 10 Nov 2023 01:47:08 GMT  
		Size: 741.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80108f24b9953bcb64ee9540cade9ebf324b97f64ec4b87c5a8bfee6fc72e43`  
		Last Modified: Fri, 10 Nov 2023 01:47:08 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bdc271cb090cd1bd78a3e982a25b3d758a4d88ba8eecb912f682acb9865621`  
		Last Modified: Fri, 10 Nov 2023 01:47:08 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfe0c9fd906a9d1d9de415579696b4e1f29d2b1006b68e6407a6612ae74aceb`  
		Last Modified: Fri, 10 Nov 2023 01:47:08 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72eb388a83e9a9a94e8b321f9b3e71ead004ac2a49ed4bc6613fa19cc76f21fe`  
		Last Modified: Fri, 10 Nov 2023 01:47:08 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.2.3`

```console
$ docker pull couchbase@sha256:df43354ee813933e1007063ac5c488001f118e8a7aeccac7aabefb472c98a7f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:7.2.3` - linux; amd64

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

### `couchbase:7.2.3` - linux; arm64 variant v8

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

## `couchbase:community`

```console
$ docker pull couchbase@sha256:f833668acb29b5470048247949ac1cf0b4402821f7866315cd8784833f769f91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:06ddc6876170c67470351fe96021fbf62d42335e84fffb8530c43d2467ae6d84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.6 MB (361636137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da27925ebd1e35b82077ebb02354d1b66dfd83333a513d672afef534d749f37e`
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
# Fri, 13 Oct 2023 07:35:15 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2
# Fri, 13 Oct 2023 07:36:55 GMT
ARG CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb
# Fri, 13 Oct 2023 07:36:55 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 13 Oct 2023 07:36:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 13 Oct 2023 07:36:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 13 Oct 2023 07:37:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=15e8e8185882210ea02ad83e3667714cce16293afad29506adf07131d684f2db            ;;          'amd64')            CB_SHA256=71bd7359e07810726c3f2735e71aa2a41e6da0865407d407bd666a3d123fa5dc            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 07:37:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 13 Oct 2023 07:37:44 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 13 Oct 2023 07:37:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 13 Oct 2023 07:37:45 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 13 Oct 2023 07:37:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 13 Oct 2023 07:37:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 13 Oct 2023 07:37:46 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 13 Oct 2023 07:37:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 Oct 2023 07:37:46 GMT
CMD ["couchbase-server"]
# Fri, 13 Oct 2023 07:37:46 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 13 Oct 2023 07:37:46 GMT
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
	-	`sha256:48ad68d41fb8b52cdd579becfb41b13f6bb57c50e22052152a2cb22cffa0a417`  
		Last Modified: Fri, 13 Oct 2023 07:46:30 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dc07baea2d8c5a6d09f65210dc95c2ececc2808487ae42d850ab86a30c92f5`  
		Last Modified: Fri, 13 Oct 2023 07:47:07 GMT  
		Size: 326.8 MB (326765101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf642dabe5c51155ff6bbf979fe616682961278cd0f3e77e0ac5e0c6964da4c5`  
		Last Modified: Fri, 13 Oct 2023 07:46:30 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27e12cfd45b43e13930af28355af4e7d1d4ae9534f5a8ea5449d3711d2c7315`  
		Last Modified: Fri, 13 Oct 2023 07:46:28 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d653d4904322fe39be1ca38d7543292f8164aa2ee366516127a833071fb70d64`  
		Last Modified: Fri, 13 Oct 2023 07:46:28 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b77eb65ad9eaabc2fb67de5df07ea736f6dae6b3d0e9abb269ed102f02fe4c`  
		Last Modified: Fri, 13 Oct 2023 07:46:28 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb108d1745d407234e8acc4a98816f489605bf3cd337a0adf0eee4312912bc2`  
		Last Modified: Fri, 13 Oct 2023 07:46:28 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa07c914f973d693531be32fd1498b96c33091c21961957b55a9790e654ae5b`  
		Last Modified: Fri, 13 Oct 2023 07:46:28 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:923561fc57c4c8c1e4219f1b9f6c19316032e43d7b7053d5c40644fbba9d761a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.2 MB (338246421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adf2613e54ef3fff2cd6f28390f34a7c6fa922c05953da8e50d391cc02c1ff7`
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
# Fri, 13 Oct 2023 03:57:09 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2
# Fri, 13 Oct 2023 03:58:28 GMT
ARG CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb
# Fri, 13 Oct 2023 03:58:28 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 13 Oct 2023 03:58:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 13 Oct 2023 03:58:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 13 Oct 2023 03:59:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=15e8e8185882210ea02ad83e3667714cce16293afad29506adf07131d684f2db            ;;          'amd64')            CB_SHA256=71bd7359e07810726c3f2735e71aa2a41e6da0865407d407bd666a3d123fa5dc            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 03:59:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 13 Oct 2023 03:59:12 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 13 Oct 2023 03:59:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 13 Oct 2023 03:59:13 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 13 Oct 2023 03:59:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 13 Oct 2023 03:59:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 13 Oct 2023 03:59:14 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 13 Oct 2023 03:59:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 Oct 2023 03:59:14 GMT
CMD ["couchbase-server"]
# Fri, 13 Oct 2023 03:59:14 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 13 Oct 2023 03:59:14 GMT
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
	-	`sha256:e6b5696b42f710080d9f3662ba9f8800b0082475f80a2a98494e3dd16eec1030`  
		Last Modified: Fri, 13 Oct 2023 04:02:38 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03702a5ff92d5a4cb798d49c06c08ab549dabd1a580175620580d957f050524`  
		Last Modified: Fri, 13 Oct 2023 04:03:06 GMT  
		Size: 304.9 MB (304932683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ff4f3347a4f58aada64b6054525cfb85dbcae59ecacc79ff9447a279b3b237`  
		Last Modified: Fri, 13 Oct 2023 04:02:38 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3aa52a8c367977e11a652b507a0c0a5d18b693ba532cc1172a70f833371c52`  
		Last Modified: Fri, 13 Oct 2023 04:02:36 GMT  
		Size: 738.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787d47784e233c5fbd08cf5aa801d9a0dba48b540524abbb2b3dddc742e53e08`  
		Last Modified: Fri, 13 Oct 2023 04:02:36 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aade2a01b48c933d14c2139bf44150d4429a89066ce89f6c9f293a134c1eae`  
		Last Modified: Fri, 13 Oct 2023 04:02:36 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4b08d5059f72202ea329c4829e56e6d3ed2878cbfc3a119abde853d994ae8e`  
		Last Modified: Fri, 13 Oct 2023 04:02:36 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7a0633784493f2f68d9b66ab5bbdde5291462cb3d44c16885b2ca536850bb9`  
		Last Modified: Fri, 13 Oct 2023 04:02:36 GMT  
		Size: 867.0 B  
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
$ docker pull couchbase@sha256:44c0ff76f625c001467f4c61b99f0784dcff42675e0420d4b50b6ed619766a8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.2` - linux; amd64

```console
$ docker pull couchbase@sha256:038ca6db1a8f6fe658a515a2c09e94b2f1074e1b70b9b6d34669e97d39e3e72b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.1 MB (429069646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4913c18e2c58e3f4b2daf2e5d3d2f857b9606177ea6663d06fee3bbb94875b`
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
# Fri, 13 Oct 2023 07:42:20 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 07:42:21 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 13 Oct 2023 07:42:21 GMT
ARG CB_VERSION=7.0.2
# Fri, 13 Oct 2023 07:42:21 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Fri, 13 Oct 2023 07:42:21 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb
# Fri, 13 Oct 2023 07:42:21 GMT
ARG CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e
# Fri, 13 Oct 2023 07:42:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 13 Oct 2023 07:42:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 13 Oct 2023 07:43:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 07:43:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 13 Oct 2023 07:43:16 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Fri, 13 Oct 2023 07:43:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 13 Oct 2023 07:43:16 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 13 Oct 2023 07:43:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 13 Oct 2023 07:43:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 13 Oct 2023 07:43:17 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 13 Oct 2023 07:43:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 Oct 2023 07:43:18 GMT
CMD ["couchbase-server"]
# Fri, 13 Oct 2023 07:43:18 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 13 Oct 2023 07:43:18 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed6f623fa5eb5d7558795b51ba0ce314182aa16c6a36192a2325018635cb61b`  
		Last Modified: Fri, 13 Oct 2023 07:50:34 GMT  
		Size: 6.3 MB (6292626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfb9a1813800ab83c9c0240f6b0d20bae58390b3cddfa5dc28766c984778605`  
		Last Modified: Fri, 13 Oct 2023 07:50:31 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c983ca90b29ff384daaab2894ca7bb190844e2a62d2f7a8dd72db4080db5a15c`  
		Last Modified: Fri, 13 Oct 2023 07:50:31 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfda45919ff0b0ec8930ec010b0af597a70fea95767c3c5cf1ad3b4a2ed9fd4`  
		Last Modified: Fri, 13 Oct 2023 07:51:16 GMT  
		Size: 394.1 MB (394062357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7987fd0b88d4087181f6694321c433289182da30be59079242ccad9a3f0d27`  
		Last Modified: Fri, 13 Oct 2023 07:50:31 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef636ad79b4564d44272b6bcc21258411cdc4910ed7c0c23b096e41f4223ae1f`  
		Last Modified: Fri, 13 Oct 2023 07:50:31 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822f6cfa4007569951b0f25fe94e19ee5c9a1b12b547028bbb2a383989dc8fcb`  
		Last Modified: Fri, 13 Oct 2023 07:50:29 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17643d71923b94b6be521715c3896429fe5bdac69e3c549706e075eb66981455`  
		Last Modified: Fri, 13 Oct 2023 07:50:29 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b193638ab47ab61e930ee556ddf47d6527e5427d02729d0150a8ae651c4b8dff`  
		Last Modified: Fri, 13 Oct 2023 07:50:29 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ccbc21f8e215691f713aea281da4354d233ebc8f55f83550b695a8f04ec578`  
		Last Modified: Fri, 13 Oct 2023 07:50:29 GMT  
		Size: 129.5 KB (129511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155fda3837d4284fafbc84649c32fef3c2c4aea3182a8d897c882861174e081a`  
		Last Modified: Fri, 13 Oct 2023 07:50:29 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.1.1`

```console
$ docker pull couchbase@sha256:4595b160f31591f5e311c9c98316f7e1d5f7a1207556b3038b85b6d7af23d257
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community-7.1.1` - linux; amd64

```console
$ docker pull couchbase@sha256:f35a8c8ec0fb150a101d76574d5342a962a78c785687bab213ca46d7a8efed77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.7 MB (346670742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b2f77305feb8d9bb40257ab93f3f3aa315ecf844c21e0b906bc0723ded83f6`
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
# Fri, 13 Oct 2023 07:39:47 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Fri, 13 Oct 2023 07:39:47 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Fri, 13 Oct 2023 07:39:47 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 13 Oct 2023 07:39:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 13 Oct 2023 07:39:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 13 Oct 2023 07:40:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 07:40:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 13 Oct 2023 07:40:35 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 13 Oct 2023 07:40:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 13 Oct 2023 07:40:36 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 13 Oct 2023 07:40:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 13 Oct 2023 07:40:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 13 Oct 2023 07:40:37 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 13 Oct 2023 07:40:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 Oct 2023 07:40:37 GMT
CMD ["couchbase-server"]
# Fri, 13 Oct 2023 07:40:37 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 13 Oct 2023 07:40:37 GMT
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
	-	`sha256:b37f0c15f08bc7e55f9e6ca8620a763529c7b3d65a30c5d0949597d2593a80ee`  
		Last Modified: Fri, 13 Oct 2023 07:48:34 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e4d54604445b14a56143ac63632cd23a514bb7b38920695509840ffb1e82b3`  
		Last Modified: Fri, 13 Oct 2023 07:49:16 GMT  
		Size: 311.8 MB (311799704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ce4b271a59b72b835e364b45ad668c9e3407731174097b6161efcb3e8e3eae`  
		Last Modified: Fri, 13 Oct 2023 07:48:34 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75f33268c189de404c41422f504290c60e1e658fd3bf82dc10587b29f8b6659`  
		Last Modified: Fri, 13 Oct 2023 07:48:32 GMT  
		Size: 742.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50be62eeac080b551ed5ccd5801dbb7c2cfca8fc1fd66254aa50df8891aa16d1`  
		Last Modified: Fri, 13 Oct 2023 07:48:33 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85c9518b0491a40a2da0ee25eb01b1ee1986d59a1d1a70646a198be408f9c42`  
		Last Modified: Fri, 13 Oct 2023 07:48:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6511d21451e2159cf1f102565ad60ccaea157c6353b06a70ed20877a0adb9e59`  
		Last Modified: Fri, 13 Oct 2023 07:48:32 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3781da98bdbd0192580a3370aa258c21c0536c2caa81ad700f564a590ddff0`  
		Last Modified: Fri, 13 Oct 2023 07:48:33 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community-7.1.1` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:2bd44ed5b21da038e43552466928607ce0be076d19d94f246e346fa8b5ecfe4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.3 MB (327340083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00ee9e21644d61a7108972820e922acc85034a2bae2c966a8cf43b07e544ac25`
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
# Fri, 13 Oct 2023 04:00:38 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Fri, 13 Oct 2023 04:00:39 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Fri, 13 Oct 2023 04:00:39 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 13 Oct 2023 04:00:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 13 Oct 2023 04:00:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 13 Oct 2023 04:01:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 04:01:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 13 Oct 2023 04:01:20 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 13 Oct 2023 04:01:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 13 Oct 2023 04:01:20 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 13 Oct 2023 04:01:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 13 Oct 2023 04:01:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 13 Oct 2023 04:01:21 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 13 Oct 2023 04:01:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 Oct 2023 04:01:22 GMT
CMD ["couchbase-server"]
# Fri, 13 Oct 2023 04:01:22 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 13 Oct 2023 04:01:22 GMT
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
	-	`sha256:d3591c2b1c95d1fb9aa0c70e363010cd4a694cd50764ae94039a2535ceeef906`  
		Last Modified: Fri, 13 Oct 2023 04:04:11 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd4da0cd2d8a9ec08c47f574c927f4de4cce610bd6e0f037a2e491b7b01a9df`  
		Last Modified: Fri, 13 Oct 2023 04:04:37 GMT  
		Size: 294.0 MB (294026335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e994d75ea102fa75ea18b3439abbdc844221889f9f3abcd148f6940679794bf4`  
		Last Modified: Fri, 13 Oct 2023 04:04:11 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde323817844aed70357ef4f5ed6f6a228e9ba71598034aa0095e87a1c2cbfb4`  
		Last Modified: Fri, 13 Oct 2023 04:04:09 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f901ca2840c4e1783b5851a1de1c250f8f3c06151ad3cd1f9045f5eecd98b`  
		Last Modified: Fri, 13 Oct 2023 04:04:09 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118f627e6b48576f25adc69ca3dc7a83171c500ca3ad800ac005e051cf0467d5`  
		Last Modified: Fri, 13 Oct 2023 04:04:09 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e99a141f7ed9aa8b9bb08d561a22a8deec5ff57cb57b0fc98c1b700043789c`  
		Last Modified: Fri, 13 Oct 2023 04:04:09 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ae9d69dddf53d974db5cdd9f470ba14c18c24ea05956e0966d06bfbcb9a4e3`  
		Last Modified: Fri, 13 Oct 2023 04:04:09 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.2.2`

```console
$ docker pull couchbase@sha256:f833668acb29b5470048247949ac1cf0b4402821f7866315cd8784833f769f91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community-7.2.2` - linux; amd64

```console
$ docker pull couchbase@sha256:06ddc6876170c67470351fe96021fbf62d42335e84fffb8530c43d2467ae6d84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.6 MB (361636137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da27925ebd1e35b82077ebb02354d1b66dfd83333a513d672afef534d749f37e`
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
# Fri, 13 Oct 2023 07:35:15 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2
# Fri, 13 Oct 2023 07:36:55 GMT
ARG CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb
# Fri, 13 Oct 2023 07:36:55 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 13 Oct 2023 07:36:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 13 Oct 2023 07:36:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 13 Oct 2023 07:37:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=15e8e8185882210ea02ad83e3667714cce16293afad29506adf07131d684f2db            ;;          'amd64')            CB_SHA256=71bd7359e07810726c3f2735e71aa2a41e6da0865407d407bd666a3d123fa5dc            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 07:37:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 13 Oct 2023 07:37:44 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 13 Oct 2023 07:37:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 13 Oct 2023 07:37:45 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 13 Oct 2023 07:37:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 13 Oct 2023 07:37:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 13 Oct 2023 07:37:46 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 13 Oct 2023 07:37:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 Oct 2023 07:37:46 GMT
CMD ["couchbase-server"]
# Fri, 13 Oct 2023 07:37:46 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 13 Oct 2023 07:37:46 GMT
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
	-	`sha256:48ad68d41fb8b52cdd579becfb41b13f6bb57c50e22052152a2cb22cffa0a417`  
		Last Modified: Fri, 13 Oct 2023 07:46:30 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dc07baea2d8c5a6d09f65210dc95c2ececc2808487ae42d850ab86a30c92f5`  
		Last Modified: Fri, 13 Oct 2023 07:47:07 GMT  
		Size: 326.8 MB (326765101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf642dabe5c51155ff6bbf979fe616682961278cd0f3e77e0ac5e0c6964da4c5`  
		Last Modified: Fri, 13 Oct 2023 07:46:30 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27e12cfd45b43e13930af28355af4e7d1d4ae9534f5a8ea5449d3711d2c7315`  
		Last Modified: Fri, 13 Oct 2023 07:46:28 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d653d4904322fe39be1ca38d7543292f8164aa2ee366516127a833071fb70d64`  
		Last Modified: Fri, 13 Oct 2023 07:46:28 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b77eb65ad9eaabc2fb67de5df07ea736f6dae6b3d0e9abb269ed102f02fe4c`  
		Last Modified: Fri, 13 Oct 2023 07:46:28 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb108d1745d407234e8acc4a98816f489605bf3cd337a0adf0eee4312912bc2`  
		Last Modified: Fri, 13 Oct 2023 07:46:28 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa07c914f973d693531be32fd1498b96c33091c21961957b55a9790e654ae5b`  
		Last Modified: Fri, 13 Oct 2023 07:46:28 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community-7.2.2` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:923561fc57c4c8c1e4219f1b9f6c19316032e43d7b7053d5c40644fbba9d761a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.2 MB (338246421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adf2613e54ef3fff2cd6f28390f34a7c6fa922c05953da8e50d391cc02c1ff7`
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
# Fri, 13 Oct 2023 03:57:09 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2
# Fri, 13 Oct 2023 03:58:28 GMT
ARG CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb
# Fri, 13 Oct 2023 03:58:28 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 13 Oct 2023 03:58:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 13 Oct 2023 03:58:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 13 Oct 2023 03:59:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=15e8e8185882210ea02ad83e3667714cce16293afad29506adf07131d684f2db            ;;          'amd64')            CB_SHA256=71bd7359e07810726c3f2735e71aa2a41e6da0865407d407bd666a3d123fa5dc            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 03:59:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 13 Oct 2023 03:59:12 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 13 Oct 2023 03:59:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 13 Oct 2023 03:59:13 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 13 Oct 2023 03:59:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 13 Oct 2023 03:59:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 13 Oct 2023 03:59:14 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 13 Oct 2023 03:59:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 Oct 2023 03:59:14 GMT
CMD ["couchbase-server"]
# Fri, 13 Oct 2023 03:59:14 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 13 Oct 2023 03:59:14 GMT
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
	-	`sha256:e6b5696b42f710080d9f3662ba9f8800b0082475f80a2a98494e3dd16eec1030`  
		Last Modified: Fri, 13 Oct 2023 04:02:38 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03702a5ff92d5a4cb798d49c06c08ab549dabd1a580175620580d957f050524`  
		Last Modified: Fri, 13 Oct 2023 04:03:06 GMT  
		Size: 304.9 MB (304932683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ff4f3347a4f58aada64b6054525cfb85dbcae59ecacc79ff9447a279b3b237`  
		Last Modified: Fri, 13 Oct 2023 04:02:38 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3aa52a8c367977e11a652b507a0c0a5d18b693ba532cc1172a70f833371c52`  
		Last Modified: Fri, 13 Oct 2023 04:02:36 GMT  
		Size: 738.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787d47784e233c5fbd08cf5aa801d9a0dba48b540524abbb2b3dddc742e53e08`  
		Last Modified: Fri, 13 Oct 2023 04:02:36 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aade2a01b48c933d14c2139bf44150d4429a89066ce89f6c9f293a134c1eae`  
		Last Modified: Fri, 13 Oct 2023 04:02:36 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4b08d5059f72202ea329c4829e56e6d3ed2878cbfc3a119abde853d994ae8e`  
		Last Modified: Fri, 13 Oct 2023 04:02:36 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7a0633784493f2f68d9b66ab5bbdde5291462cb3d44c16885b2ca536850bb9`  
		Last Modified: Fri, 13 Oct 2023 04:02:36 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:df43354ee813933e1007063ac5c488001f118e8a7aeccac7aabefb472c98a7f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise` - linux; amd64

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

### `couchbase:enterprise` - linux; arm64 variant v8

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

## `couchbase:enterprise-6.6.6`

```console
$ docker pull couchbase@sha256:9de84627fcb614ffdea20e08bd070e81fb606572bf61df8a316d5677a6619d4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.6` - linux; amd64

```console
$ docker pull couchbase@sha256:84ef86645157a156d758d33832b3a49c1339b1d77702eb3278778917c02bde2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.0 MB (532020334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58ad678e9ec231c108ae4761d227f4d469ff29c0ef7ba5b742fafca6b746df24`
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
# Fri, 13 Oct 2023 07:43:33 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6
# Fri, 13 Oct 2023 07:43:33 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb
# Fri, 13 Oct 2023 07:43:33 GMT
ARG CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa
# Fri, 13 Oct 2023 07:43:33 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 13 Oct 2023 07:43:34 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Fri, 13 Oct 2023 07:43:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 13 Oct 2023 07:43:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 13 Oct 2023 07:44:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 07:44:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 13 Oct 2023 07:44:39 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 13 Oct 2023 07:44:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 13 Oct 2023 07:44:40 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 13 Oct 2023 07:44:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 13 Oct 2023 07:44:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 13 Oct 2023 07:44:41 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 13 Oct 2023 07:44:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 Oct 2023 07:44:41 GMT
CMD ["couchbase-server"]
# Fri, 13 Oct 2023 07:44:41 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 13 Oct 2023 07:44:41 GMT
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
	-	`sha256:99f6de63974d9b749570af50a3746b675e45e5a8a4650f036fdb34d46e18c2b6`  
		Last Modified: Fri, 13 Oct 2023 07:51:25 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00c4a58175bb4f00cd56f289b18fece37016bb4c2a1d645af19e9665ade0592`  
		Last Modified: Fri, 13 Oct 2023 07:52:12 GMT  
		Size: 497.1 MB (497149289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f391182a481ef73a0c0ab3a6024b5a69b7f21b98474db4040a67f661f6421055`  
		Last Modified: Fri, 13 Oct 2023 07:51:25 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e649472c0f465231e1c5718cc5c3a5cbf96b1715fdf7efc7008b33040def055`  
		Last Modified: Fri, 13 Oct 2023 07:51:23 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f56fe0b9735a33cf3be6fc48a578d90f03a69715a28c066e4be7e78fc1d16f4`  
		Last Modified: Fri, 13 Oct 2023 07:51:23 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820aec2c4f3736feee2c2c0dc7e84d72efed62e50f3e9cf8e1eb826e12e6d6ad`  
		Last Modified: Fri, 13 Oct 2023 07:51:23 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e1af6b7af088fedb4895f19c17168df7af26bfd525a38e08ebe0b4667ce89e`  
		Last Modified: Fri, 13 Oct 2023 07:51:23 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0213a0b01f3c015fec705d9c2c220710d158d3111b8bf28d1bba01b0f775d01b`  
		Last Modified: Fri, 13 Oct 2023 07:51:23 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.0.5`

```console
$ docker pull couchbase@sha256:5d9823c688107551d0f4153de5e98505d0fb2b3d3bb99b7a619a84d04ba381dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:2ebdb38bf4f0c3330c205f1966779479e562cf8f51cf803a26cc352a5cfddcfc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **616.7 MB (616700956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e1d1e932031b1b0c647cd28688b4afd7e9dcbaba460f0e9ed3add403e5ccee9`
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
# Fri, 13 Oct 2023 07:40:46 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5
# Fri, 13 Oct 2023 07:40:46 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb
# Fri, 13 Oct 2023 07:40:46 GMT
ARG CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea
# Fri, 13 Oct 2023 07:40:46 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 13 Oct 2023 07:40:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 13 Oct 2023 07:40:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 13 Oct 2023 07:42:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 13 Oct 2023 07:42:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 13 Oct 2023 07:42:05 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 13 Oct 2023 07:42:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 13 Oct 2023 07:42:05 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 13 Oct 2023 07:42:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 13 Oct 2023 07:42:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 13 Oct 2023 07:42:06 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 13 Oct 2023 07:42:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 Oct 2023 07:42:06 GMT
CMD ["couchbase-server"]
# Fri, 13 Oct 2023 07:42:07 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 13 Oct 2023 07:42:07 GMT
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
	-	`sha256:17d7d10e9d142fc70e227ceb9b178daa7d79ed36af0d26b176229999a2a2150f`  
		Last Modified: Fri, 13 Oct 2023 07:49:25 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24925c079cdf75fc52f3b3c4109e3dba2f5ed77320285c527cfedbc869814bef`  
		Last Modified: Fri, 13 Oct 2023 07:50:20 GMT  
		Size: 581.8 MB (581829904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51dcd503c527731a115e4b5da8f216756ba95d790c44153fb87f6c2e11c0a48`  
		Last Modified: Fri, 13 Oct 2023 07:49:25 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6686a51b4d13ae5b4e3f21385169b8790ce2a83eedca61e7f61a51e527c5e5f`  
		Last Modified: Fri, 13 Oct 2023 07:49:23 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b623a9e24470a10dbd831afc95ff0571b572ccde3bae1061906f25b42cf3867b`  
		Last Modified: Fri, 13 Oct 2023 07:49:23 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0314f2c61a2ca1bd2420f1293e60988fd014cc10ab4851519cb5f433421eae`  
		Last Modified: Fri, 13 Oct 2023 07:49:23 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7c453d64636975972288cc988cffe3f17c944292b1c2e16991de1c6ee18b87`  
		Last Modified: Fri, 13 Oct 2023 07:49:23 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0d7d5fe83e5abaf9456d1635b34f428ab51bb36406817a6509f88d150a6723`  
		Last Modified: Fri, 13 Oct 2023 07:49:23 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.1.6`

```console
$ docker pull couchbase@sha256:8e0421be746581ad8e1c32560c5dad18bcb1dc4129b35ab40126e90d94e9b334
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise-7.1.6` - linux; amd64

```console
$ docker pull couchbase@sha256:af6fc4ac2462e4133102e9730fc574cffe857d94ab140b2548d77fc5ecf1ba8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **652.0 MB (652019059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e313655605252ec475e3270221b3d975ac35c9d9ce30934f642e24026141cc`
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
# Fri, 10 Nov 2023 02:31:29 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6
# Fri, 10 Nov 2023 02:31:29 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb
# Fri, 10 Nov 2023 02:31:29 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 10 Nov 2023 02:31:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 10 Nov 2023 02:31:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 10 Nov 2023 02:32:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=d4462e7228c372f761bd83f96fa63a7211544df885c2d2e065202ff663dad6f9            ;;          'amd64')            CB_SHA256=abf410a1f97dd14171cd260d4abb853be003db5ec0a44c8324c846068eb90ce7            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 10 Nov 2023 02:32:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 10 Nov 2023 02:32:57 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 10 Nov 2023 02:32:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 10 Nov 2023 02:32:57 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 10 Nov 2023 02:32:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 10 Nov 2023 02:32:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 10 Nov 2023 02:32:59 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 10 Nov 2023 02:32:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Nov 2023 02:32:59 GMT
CMD ["couchbase-server"]
# Fri, 10 Nov 2023 02:32:59 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 10 Nov 2023 02:32:59 GMT
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
	-	`sha256:191174dc2fdae0ccd3b590fde88f3415924e068016cdf948f131cf67739d2628`  
		Last Modified: Fri, 10 Nov 2023 02:34:55 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8872eee949d51c285aeea4e66f04b56279ecd305ba93f9551e368445497d4c36`  
		Last Modified: Fri, 10 Nov 2023 02:35:57 GMT  
		Size: 617.1 MB (617148011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e0a1b755ccc9a7b525bdb0186c60807f93bf4ed5f09dbbc785096109b579bd`  
		Last Modified: Fri, 10 Nov 2023 02:34:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7204d59c585c6547badfc9c91d84d8a0002f4bf842493cdce761cbf11dee64a`  
		Last Modified: Fri, 10 Nov 2023 02:34:53 GMT  
		Size: 746.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab274fa467540d702716aa6838c1c890cb5be73c83023320c99805b278d53c8d`  
		Last Modified: Fri, 10 Nov 2023 02:34:53 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23319a23df40d9ce4ae83364f0ec90b745b0af326da752510c43d1fb22d93c8`  
		Last Modified: Fri, 10 Nov 2023 02:34:53 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef7150892bce389f2c09c0218a3c88ebfabc41aebe6938334085f0380766cd6`  
		Last Modified: Fri, 10 Nov 2023 02:34:53 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71806bdbdb06e7ca1d154faeae1a670d05527fbe56c7455f976b0e445ebfb073`  
		Last Modified: Fri, 10 Nov 2023 02:34:53 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:enterprise-7.1.6` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:458dff220edcf4672b52fdc4677dc268a4e8175a259f66cc3f0119e9abe00fbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **622.6 MB (622639193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:023645d7f36f8e44a98a6f71839d814535388b15c3a6c2bf3fca3cd298a32f4c`
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
# Fri, 10 Nov 2023 01:44:34 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6
# Fri, 10 Nov 2023 01:44:34 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb
# Fri, 10 Nov 2023 01:44:34 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 10 Nov 2023 01:44:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 10 Nov 2023 01:44:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 10 Nov 2023 01:45:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=d4462e7228c372f761bd83f96fa63a7211544df885c2d2e065202ff663dad6f9            ;;          'amd64')            CB_SHA256=abf410a1f97dd14171cd260d4abb853be003db5ec0a44c8324c846068eb90ce7            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 10 Nov 2023 01:45:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 10 Nov 2023 01:45:44 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 10 Nov 2023 01:45:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 10 Nov 2023 01:45:45 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 10 Nov 2023 01:45:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 10 Nov 2023 01:45:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.6-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 10 Nov 2023 01:45:46 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 10 Nov 2023 01:45:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Nov 2023 01:45:46 GMT
CMD ["couchbase-server"]
# Fri, 10 Nov 2023 01:45:46 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 10 Nov 2023 01:45:46 GMT
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
	-	`sha256:4ffda5421b450b5fe26e86864039e1f859621548c5a669a0e07b276fdecebcc4`  
		Last Modified: Fri, 10 Nov 2023 01:47:11 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c02dc935d32efcc9648883ef289c3db68ac3a67d804069d2fd6da95170127aa`  
		Last Modified: Fri, 10 Nov 2023 01:47:50 GMT  
		Size: 589.3 MB (589325444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d59fcdd23df8ac9d0371fb1b7c95b21632a816f14a642ecdad59153b84a83b`  
		Last Modified: Fri, 10 Nov 2023 01:47:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2a5301f374b0a3d811ab6a096485c45de7688a642c383a6fb7f21864840b04`  
		Last Modified: Fri, 10 Nov 2023 01:47:08 GMT  
		Size: 741.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80108f24b9953bcb64ee9540cade9ebf324b97f64ec4b87c5a8bfee6fc72e43`  
		Last Modified: Fri, 10 Nov 2023 01:47:08 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bdc271cb090cd1bd78a3e982a25b3d758a4d88ba8eecb912f682acb9865621`  
		Last Modified: Fri, 10 Nov 2023 01:47:08 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfe0c9fd906a9d1d9de415579696b4e1f29d2b1006b68e6407a6612ae74aceb`  
		Last Modified: Fri, 10 Nov 2023 01:47:08 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72eb388a83e9a9a94e8b321f9b3e71ead004ac2a49ed4bc6613fa19cc76f21fe`  
		Last Modified: Fri, 10 Nov 2023 01:47:08 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:df43354ee813933e1007063ac5c488001f118e8a7aeccac7aabefb472c98a7f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:latest` - linux; amd64

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

### `couchbase:latest` - linux; arm64 variant v8

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
