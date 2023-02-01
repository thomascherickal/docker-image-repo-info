<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchbase`

-	[`couchbase:6.6.6`](#couchbase666)
-	[`couchbase:7.0.5`](#couchbase705)
-	[`couchbase:7.1.3`](#couchbase713)
-	[`couchbase:community`](#couchbasecommunity)
-	[`couchbase:community-6.6.0`](#couchbasecommunity-660)
-	[`couchbase:community-7.0.2`](#couchbasecommunity-702)
-	[`couchbase:community-7.1.1`](#couchbasecommunity-711)
-	[`couchbase:enterprise`](#couchbaseenterprise)
-	[`couchbase:enterprise-6.6.6`](#couchbaseenterprise-666)
-	[`couchbase:enterprise-7.0.5`](#couchbaseenterprise-705)
-	[`couchbase:enterprise-7.1.3`](#couchbaseenterprise-713)
-	[`couchbase:latest`](#couchbaselatest)

## `couchbase:6.6.6`

```console
$ docker pull couchbase@sha256:6f81f5e905693699c40d748fc87a55b33373f7707f34ba62a4081b89c4ff9c8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.6` - linux; amd64

```console
$ docker pull couchbase@sha256:732324fc9d9f651f81b9f71a856a7626ab1dd8a43d125082cb9661e657dc2cf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.9 MB (531947740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cb9fb9b73bc5e125f3c752235b67f567c89cd23ba831d1f04a463bc7db37233`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:25:04 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:25:04 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:25:04 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:25:27 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:29:49 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6
# Wed, 01 Feb 2023 18:29:49 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb
# Wed, 01 Feb 2023 18:29:49 GMT
ARG CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa
# Wed, 01 Feb 2023 18:29:49 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:29:49 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Wed, 01 Feb 2023 18:29:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:29:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:30:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:30:42 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:30:42 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:30:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:30:43 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:30:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:30:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:30:44 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:30:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:30:44 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:30:44 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:30:44 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b4cf586c4b7a57fc5e73b3aa283d12081f9bd7606b6b60d897f2783e6efa0d`  
		Last Modified: Wed, 01 Feb 2023 18:31:06 GMT  
		Size: 6.2 MB (6216449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5740863927d97994ec3d21c6de0af467b0ae510d8b0293c8e74c73ec07f5ae0`  
		Last Modified: Wed, 01 Feb 2023 18:35:13 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d164b95c54f4b3fdd0d6e30b6d600d3915718d54a8bf5253c84358ef7c72a5`  
		Last Modified: Wed, 01 Feb 2023 18:36:03 GMT  
		Size: 497.1 MB (497149037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c584dbdd2a7bd3addb8f233ef50d596406de06899eee48d88dcd761f842a320`  
		Last Modified: Wed, 01 Feb 2023 18:35:13 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8fa8bc7de4e50e414cb9a0484780220be102116142d15bfb0224867be0d6a1`  
		Last Modified: Wed, 01 Feb 2023 18:35:11 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0bc4a117c18c99798b1f51f2240a6ce57140c30f471c903b58f1adf772b0b8`  
		Last Modified: Wed, 01 Feb 2023 18:35:11 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e70f25ba12d1bcccb97dad4d9b8a50645d0b1a8ef7bcb0247abb2232e5634a`  
		Last Modified: Wed, 01 Feb 2023 18:35:11 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ec254ae18d152e1db206ddc4668eae893cc6dae5b8cbea0f8e2dba7e52328c`  
		Last Modified: Wed, 01 Feb 2023 18:35:11 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cfb26fc8248bff887d3cde118fa5b5c41d9cb9904b7710823c1b7c1a5f947`  
		Last Modified: Wed, 01 Feb 2023 18:35:11 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.0.5`

```console
$ docker pull couchbase@sha256:70d1600c289c834e69caaea2c8c981b5a9ebc245e91d6d729bd333e77f95c072
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:7.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:afa70468149f42aa257d2fdc35c6b4d748dfe077abd7f101a040ec5080b119d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **616.6 MB (616628710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c670efa3cc51d5c7a1ae1bef657131d726a397c150d225219e0593613b5dc0e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:25:04 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:25:04 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:25:04 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:25:27 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:27:30 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5
# Wed, 01 Feb 2023 18:27:30 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb
# Wed, 01 Feb 2023 18:27:31 GMT
ARG CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea
# Wed, 01 Feb 2023 18:27:31 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:27:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:27:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:28:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:28:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:28:31 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:28:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:28:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:28:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:28:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:28:33 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:28:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:28:33 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:28:33 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:28:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b4cf586c4b7a57fc5e73b3aa283d12081f9bd7606b6b60d897f2783e6efa0d`  
		Last Modified: Wed, 01 Feb 2023 18:31:06 GMT  
		Size: 6.2 MB (6216449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507b7a7e538510c11f6158504c6a0cc9e16b8dd599ac2f8515b103b246de8e21`  
		Last Modified: Wed, 01 Feb 2023 18:33:05 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de73b439ff8a91b36710c23edc8ca56c4e921ef41b2e6cb71224ea3b546b3aa`  
		Last Modified: Wed, 01 Feb 2023 18:34:03 GMT  
		Size: 581.8 MB (581830013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0738cfd3ccb6b0abfd4708b88a453af4c05a739ed6058036452db84dd98c54`  
		Last Modified: Wed, 01 Feb 2023 18:33:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81320e19b263a40ecbae84dfcba6bd77c9d19dcb14dc1b9633db54316234e955`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 741.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5e61bf65fb7021f8f7fd08cc267e9e3d2bab7e16ead1a46300ae4fa8bd4fe0`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d065117ea502454506cbd8e4c642c1a45641130b86465e564daa4dade7b495a`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ef5abe6b3270b049506d26a9c2b97d6470bdd23f5004da355c317a9e076005`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85caa0ee6487d6e3f055aa6ccb1420be7f7e05020ab26456a63a9fe63b655b62`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.1.3`

```console
$ docker pull couchbase@sha256:0da3172d19deeb8eb825ed8a84c407710833f767f0778f048b08e7a460e58bf4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:7.1.3` - linux; amd64

```console
$ docker pull couchbase@sha256:27442f3b0200d77b37168f5687f30e2a999947ef0a5db598c4750e97fb92e3d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **600.3 MB (600285393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5ec1dd33ec9082d8c2d7e9a150579b5193c1f6d18df628b4decf3bec9209055`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:25:04 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:25:04 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:25:04 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:25:27 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:25:28 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3
# Wed, 01 Feb 2023 18:25:28 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb
# Wed, 01 Feb 2023 18:25:28 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:25:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:25:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:26:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=bdc1ffbd5a0eca07a554856a92eb0b5930b457c1d13fca9a2a93ef91a5d88156            ;;          'amd64')            CB_SHA256=bd8c808771cb46e563c173f60e0723c32351a6453f6ece2d4fa440e0d2dcdfd3            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:26:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:26:31 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:26:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:26:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:26:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:26:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:26:33 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:26:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:26:33 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:26:33 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:26:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b4cf586c4b7a57fc5e73b3aa283d12081f9bd7606b6b60d897f2783e6efa0d`  
		Last Modified: Wed, 01 Feb 2023 18:31:06 GMT  
		Size: 6.2 MB (6216449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2820c7121f0a09d4a6b11881f09b95cacc3cbebc82f73aff1f996202193ce0`  
		Last Modified: Wed, 01 Feb 2023 18:31:05 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db5dca17b86b88c0c7cf2b23d43c1ed0561f66106e0b0a955667da1dc1401`  
		Last Modified: Wed, 01 Feb 2023 18:32:01 GMT  
		Size: 565.5 MB (565486707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d11bb0b33cc4ea595033a41004eeea233f267374a44a5dc97bd226bcb64e0d8`  
		Last Modified: Wed, 01 Feb 2023 18:31:05 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a801c20d9d04c9fffd9c9584e4383bf75463ec98280eb032175223dfb87f1980`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 739.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2988e82038abb9d711b27510974291e14223e2834c95c920ce5938a6e7a2c2c`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35420a0cd22388f3cc77425bfc3f5d128433747095ebac6d391c01742be295c`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bea392911ee85dcff4c4d9224495188208fa48c7c4022a52c08b7788dad184`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe9dae4957e5be3f0645755f477cb900b50908d1d7587c4ff46ab294f41d8e4`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:7.1.3` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:3c4cabfcbeead72e9ce88f6051d46a67adeeb7b6c16799531b60712cb35c3a4b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.4 MB (574395108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5d8125b01452ee161b3c515386eb7ed92cafd6950fe5e0fad033a50d4dd2b7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:17:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:17:34 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:17:34 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:17:53 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:17:54 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3
# Wed, 01 Feb 2023 18:17:54 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb
# Wed, 01 Feb 2023 18:17:54 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:17:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:17:54 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:18:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=bdc1ffbd5a0eca07a554856a92eb0b5930b457c1d13fca9a2a93ef91a5d88156            ;;          'amd64')            CB_SHA256=bd8c808771cb46e563c173f60e0723c32351a6453f6ece2d4fa440e0d2dcdfd3            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:18:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:18:46 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:18:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:18:47 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:18:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:18:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:18:48 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:18:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:18:48 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:18:48 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:18:48 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df4acc3280127d63542436253f90f4862c9daaef8ed9ea6e07468221a331164`  
		Last Modified: Wed, 01 Feb 2023 18:19:49 GMT  
		Size: 6.0 MB (6039600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56507591370d4d0a4f9266f6983fc882e469e4c9e18638607ebcd310f752bee`  
		Last Modified: Wed, 01 Feb 2023 18:19:48 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e665174c1121b08e9cbfe29177246dd777f3e9f7f7222abbda480985d136c9`  
		Last Modified: Wed, 01 Feb 2023 18:20:29 GMT  
		Size: 541.2 MB (541157405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed85a620835a4af7f402e88ce29f4abe542cb789ee87df6ac7513ae079e815b`  
		Last Modified: Wed, 01 Feb 2023 18:19:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a08982e57dc712bd074870be2d27ccac43380110e21f0a57ea08ee47e34eaf2`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8faa6408783f533b1322b793f5af9800d0ec262eb2fa039646f2587c969500f`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9cd106ccd30da4072a96b97d251a59e8fb9fdf30cf9ad2b3a7910759145851`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2337915ae138787ede0fb08dca68b24dcb59dc626bdda5fe902b142896f7919a`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11379d1c166bf612fc0e058e00faa700dcae528cbff06925c1fe5394db7f0b46`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community`

```console
$ docker pull couchbase@sha256:7c2a3971ff14ca59528864781ec96ceaeae508a309caa4574221858c17fd0c34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:c9f4154e895e8574268027d046fe7f12a9a59ff9a7365b90854f19d1c124e4cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.6 MB (346597781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39220a3e298986d8513e334800e17c4585c93882a28b810d92c5fc1c0c7994e9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:25:04 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:25:04 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:25:04 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:25:27 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:26:42 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Wed, 01 Feb 2023 18:26:42 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Wed, 01 Feb 2023 18:26:42 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:26:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:26:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:27:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:27:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:27:21 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:27:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:27:21 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:27:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:27:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:27:23 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:27:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:27:23 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:27:23 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 01 Feb 2023 18:27:23 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b4cf586c4b7a57fc5e73b3aa283d12081f9bd7606b6b60d897f2783e6efa0d`  
		Last Modified: Wed, 01 Feb 2023 18:31:06 GMT  
		Size: 6.2 MB (6216449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9104ac5883bac220a5f574ba7966f482cea80896107af366ff3070096269b6d8`  
		Last Modified: Wed, 01 Feb 2023 18:32:16 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5badd907bdc9e401e76b24e9f00dae2ce8a147ba07a3318b7db146c942e634`  
		Last Modified: Wed, 01 Feb 2023 18:32:54 GMT  
		Size: 311.8 MB (311799081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24350a0cac3b682c873ae27c1e4e99a3a230d8f463d6fc41c789afabb9e253d9`  
		Last Modified: Wed, 01 Feb 2023 18:32:16 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ae8adb8b33072989ccd8b1bb270ce6dc12ac81b9bbcd9297cb9b16ebcb67ce`  
		Last Modified: Wed, 01 Feb 2023 18:32:14 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46fc231003be1da0d19984c4d4bf1cfc24878eded7c73c8029c2bc643dbe657`  
		Last Modified: Wed, 01 Feb 2023 18:32:15 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8449d72ddff01b8dc6be535e0cd417fd17845f9562e0371190882071d997235b`  
		Last Modified: Wed, 01 Feb 2023 18:32:15 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaea83304a41aaa60679eb036b0aa0052a0e345e8732f4f98f0ba110e3d63626`  
		Last Modified: Wed, 01 Feb 2023 18:32:14 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fad92e762b2a92e079e8c6da1631613fb22d047a081feddbac24d190eedc20`  
		Last Modified: Wed, 01 Feb 2023 18:32:15 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:777953812d33a1fb326bc99ea87ab5b5b0fb627787ee179aa8d4f9fcb07a72c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.3 MB (327262891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f95a94f743a4f7a77036989ec8c29457d286cccf603a064ef2fd270b13dab04c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:17:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:17:34 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:17:34 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:17:53 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:18:57 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Wed, 01 Feb 2023 18:18:57 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Wed, 01 Feb 2023 18:18:57 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:18:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:18:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:19:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:19:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:19:30 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:19:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:19:30 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:19:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:19:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:19:32 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:19:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:19:32 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:19:32 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 01 Feb 2023 18:19:32 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df4acc3280127d63542436253f90f4862c9daaef8ed9ea6e07468221a331164`  
		Last Modified: Wed, 01 Feb 2023 18:19:49 GMT  
		Size: 6.0 MB (6039600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6618b315b476a367a7a71a3a2a93e148dafe6c7ffe372de6e9ed1f403e7928`  
		Last Modified: Wed, 01 Feb 2023 18:20:44 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3717b8c3a4f260615b5cb089d3bae702b9eb60bfe6b13e67d0f6eccab00d5e`  
		Last Modified: Wed, 01 Feb 2023 18:21:11 GMT  
		Size: 294.0 MB (294025193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2ef92333e89f2209138091cccae62a07d1f2b59b38d6f65701f9e043104a53`  
		Last Modified: Wed, 01 Feb 2023 18:20:44 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4651ae91c1ab8af36a2800b9b5eb3cb08c5a13cf19fe563aae1fc1d13be8833`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 739.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18665cd1d0000877ad3ef689d96d10bb43c098dff34717b0e17ac9d04ef5ace`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4c94998c413cc533560b47d6afac69ebdc6037cff2dabf530a90135d980ede`  
		Last Modified: Wed, 01 Feb 2023 18:20:43 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d3f1cbafefcfd0a5136a2f172055fb2c456d491320719ae320e3e8e71771bd`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28f154ea67856aa73cfde3cd5bacfa7b5821994cc62f7aa9c393b19c2eeafbf`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:86b73a3ff841e3794e842917965e6d4cc160d9b0adaca49f76647526059a4cc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:171ee8e5ce62a812392b85cad555f8003aa6174e6072b82ff2b23b1c9c410c5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.5 MB (352518630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16a0f064a9d5ce44434a2f66a3032b823f7b7d8e03897f1bee34b05c2c0726b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:12:14 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 31 Jan 2023 18:12:14 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Tue, 31 Jan 2023 18:12:14 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Jan 2023 18:12:40 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Tue, 31 Jan 2023 18:12:40 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Tue, 31 Jan 2023 18:12:40 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb
# Tue, 31 Jan 2023 18:12:40 GMT
ARG CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559
# Tue, 31 Jan 2023 18:12:40 GMT
ARG CB_SKIP_CHECKSUM=false
# Tue, 31 Jan 2023 18:12:40 GMT
ARG CB_PACKAGE_NAME=couchbase-server-community
# Tue, 31 Jan 2023 18:12:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 31 Jan 2023 18:12:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 31 Jan 2023 18:13:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server-community     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Tue, 31 Jan 2023 18:13:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 31 Jan 2023 18:13:22 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Tue, 31 Jan 2023 18:13:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 31 Jan 2023 18:13:23 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 31 Jan 2023 18:13:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 31 Jan 2023 18:13:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Tue, 31 Jan 2023 18:13:32 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Tue, 31 Jan 2023 18:13:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Jan 2023 18:13:32 GMT
CMD ["couchbase-server"]
# Tue, 31 Jan 2023 18:13:32 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 31 Jan 2023 18:13:32 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66777604cfa2ea3a3dc8d9f4abc45b1837ba541d9d1f652cd6240bafe76e7ad7`  
		Last Modified: Tue, 31 Jan 2023 18:19:00 GMT  
		Size: 5.6 MB (5606095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bd6fa8d41e1f214d2c08918573af687bb87d5ae9d6a38e9ad79214c0d6fdef`  
		Last Modified: Tue, 31 Jan 2023 18:18:59 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce91435633be772959fb2884206892925de4353c52b7919b30dbc1948adba630`  
		Last Modified: Tue, 31 Jan 2023 18:19:33 GMT  
		Size: 319.8 MB (319763168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bae63f5766d12b7eaa20e78ce08818a2efb76a30a6a9026f659f362a9e4139`  
		Last Modified: Tue, 31 Jan 2023 18:18:59 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f656acc8afbaa77aa0dca0b3cfdd9a1c11ed3d2baf9eb8b0f39300518549f76`  
		Last Modified: Tue, 31 Jan 2023 18:18:59 GMT  
		Size: 741.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecb255262042521b0fc4e7f716636e9e83de72a6f7a709004bca3f49d310d87`  
		Last Modified: Tue, 31 Jan 2023 18:18:57 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07617d77fb8bf57652ed9585f1708bfb9e94761e324c13ec0ab636b01d89ee0`  
		Last Modified: Tue, 31 Jan 2023 18:18:57 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c20e7ed7236744b51c5bb879ea806c3077c89b6e896a24bcc3eb290ec8fee75`  
		Last Modified: Tue, 31 Jan 2023 18:18:57 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ce2b034ccbdc95402f381869213fad50d20d026fbea471b6ba317f27f10d6e`  
		Last Modified: Tue, 31 Jan 2023 18:18:57 GMT  
		Size: 433.3 KB (433280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6229f835e3e3c7a7beedae40f3c73f39245a5f9f96f3e9cecc7fcaf0b428cc4e`  
		Last Modified: Tue, 31 Jan 2023 18:18:57 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.0.2`

```console
$ docker pull couchbase@sha256:9a78cd01ec6d0909152d837a3e73db5ed2731addab8b44caed844b737a43d57a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.2` - linux; amd64

```console
$ docker pull couchbase@sha256:0bb66f31144c218710ff8e170b21fe0bc9dec9f4a25b0811a8bc29db3dd29daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.0 MB (428997524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:603eef5729ca89a5a1267bf26c28764b0fed80c6f35ce5b241562606c092dfe4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:25:04 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:28:50 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:28:50 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 01 Feb 2023 18:28:50 GMT
ARG CB_VERSION=7.0.2
# Wed, 01 Feb 2023 18:28:51 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Wed, 01 Feb 2023 18:28:51 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb
# Wed, 01 Feb 2023 18:28:51 GMT
ARG CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e
# Wed, 01 Feb 2023 18:28:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:28:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:29:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:29:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:29:39 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:29:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:29:40 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:29:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:29:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 01 Feb 2023 18:29:41 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 01 Feb 2023 18:29:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:29:41 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:29:41 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 01 Feb 2023 18:29:41 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87459cb81c69946d85cb34faad4bcd6f0be251f84a5862aed8dad66fbd4efcb8`  
		Last Modified: Wed, 01 Feb 2023 18:34:17 GMT  
		Size: 6.2 MB (6223751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e8f4cc124b9cb1cca9952b2b70adc22d91677992ec2494c6ccc4dbcaac1e8a`  
		Last Modified: Wed, 01 Feb 2023 18:34:14 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f18a967de7966d3413a9556f799a2437c1dedd00f5863af5c6add5d3e7e5a5e`  
		Last Modified: Wed, 01 Feb 2023 18:34:14 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53613a6321909a2fb934242f3104283929ada51275ca7624efdc27ebec391449`  
		Last Modified: Wed, 01 Feb 2023 18:35:04 GMT  
		Size: 394.1 MB (394061895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac787b92751032e322e37f6274e4725fa46c7d4430db829b26619a4ab27c6311`  
		Last Modified: Wed, 01 Feb 2023 18:34:15 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e373f51018053af39a7e3e4a7d6fb3c7c2ff005f7ef29d6ffae83c45f36ced`  
		Last Modified: Wed, 01 Feb 2023 18:34:14 GMT  
		Size: 604.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ddadf9276cd1695f611ede0c65ec2710f47f8b070ae0323943ed4f65bf2ae3`  
		Last Modified: Wed, 01 Feb 2023 18:34:12 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9d54354d18cc739659f905bf2a2debbaf66c0c0a9c1885f7ec136bb4cf1df7`  
		Last Modified: Wed, 01 Feb 2023 18:34:12 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d653a74a9994f37477a2d148c5aeae793a7156874482e1efbb0e2b2b4d294ffb`  
		Last Modified: Wed, 01 Feb 2023 18:34:12 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4047d0fb1040c55defec7de0388c1293f5f864aa6939e72f7c2e1073fe38341b`  
		Last Modified: Wed, 01 Feb 2023 18:34:12 GMT  
		Size: 129.5 KB (129509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2138c4e7404f0a2ac26c0e0836175bd1b2a80cea89a51bfd242ca90823542bc9`  
		Last Modified: Wed, 01 Feb 2023 18:34:12 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.1.1`

```console
$ docker pull couchbase@sha256:7c2a3971ff14ca59528864781ec96ceaeae508a309caa4574221858c17fd0c34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community-7.1.1` - linux; amd64

```console
$ docker pull couchbase@sha256:c9f4154e895e8574268027d046fe7f12a9a59ff9a7365b90854f19d1c124e4cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.6 MB (346597781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39220a3e298986d8513e334800e17c4585c93882a28b810d92c5fc1c0c7994e9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:25:04 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:25:04 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:25:04 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:25:27 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:26:42 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Wed, 01 Feb 2023 18:26:42 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Wed, 01 Feb 2023 18:26:42 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:26:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:26:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:27:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:27:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:27:21 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:27:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:27:21 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:27:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:27:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:27:23 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:27:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:27:23 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:27:23 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 01 Feb 2023 18:27:23 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b4cf586c4b7a57fc5e73b3aa283d12081f9bd7606b6b60d897f2783e6efa0d`  
		Last Modified: Wed, 01 Feb 2023 18:31:06 GMT  
		Size: 6.2 MB (6216449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9104ac5883bac220a5f574ba7966f482cea80896107af366ff3070096269b6d8`  
		Last Modified: Wed, 01 Feb 2023 18:32:16 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5badd907bdc9e401e76b24e9f00dae2ce8a147ba07a3318b7db146c942e634`  
		Last Modified: Wed, 01 Feb 2023 18:32:54 GMT  
		Size: 311.8 MB (311799081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24350a0cac3b682c873ae27c1e4e99a3a230d8f463d6fc41c789afabb9e253d9`  
		Last Modified: Wed, 01 Feb 2023 18:32:16 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ae8adb8b33072989ccd8b1bb270ce6dc12ac81b9bbcd9297cb9b16ebcb67ce`  
		Last Modified: Wed, 01 Feb 2023 18:32:14 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46fc231003be1da0d19984c4d4bf1cfc24878eded7c73c8029c2bc643dbe657`  
		Last Modified: Wed, 01 Feb 2023 18:32:15 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8449d72ddff01b8dc6be535e0cd417fd17845f9562e0371190882071d997235b`  
		Last Modified: Wed, 01 Feb 2023 18:32:15 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaea83304a41aaa60679eb036b0aa0052a0e345e8732f4f98f0ba110e3d63626`  
		Last Modified: Wed, 01 Feb 2023 18:32:14 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fad92e762b2a92e079e8c6da1631613fb22d047a081feddbac24d190eedc20`  
		Last Modified: Wed, 01 Feb 2023 18:32:15 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community-7.1.1` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:777953812d33a1fb326bc99ea87ab5b5b0fb627787ee179aa8d4f9fcb07a72c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.3 MB (327262891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f95a94f743a4f7a77036989ec8c29457d286cccf603a064ef2fd270b13dab04c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:17:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:17:34 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:17:34 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:17:53 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:18:57 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Wed, 01 Feb 2023 18:18:57 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Wed, 01 Feb 2023 18:18:57 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:18:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:18:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:19:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:19:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:19:30 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:19:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:19:30 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:19:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:19:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:19:32 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:19:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:19:32 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:19:32 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 01 Feb 2023 18:19:32 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df4acc3280127d63542436253f90f4862c9daaef8ed9ea6e07468221a331164`  
		Last Modified: Wed, 01 Feb 2023 18:19:49 GMT  
		Size: 6.0 MB (6039600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6618b315b476a367a7a71a3a2a93e148dafe6c7ffe372de6e9ed1f403e7928`  
		Last Modified: Wed, 01 Feb 2023 18:20:44 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3717b8c3a4f260615b5cb089d3bae702b9eb60bfe6b13e67d0f6eccab00d5e`  
		Last Modified: Wed, 01 Feb 2023 18:21:11 GMT  
		Size: 294.0 MB (294025193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2ef92333e89f2209138091cccae62a07d1f2b59b38d6f65701f9e043104a53`  
		Last Modified: Wed, 01 Feb 2023 18:20:44 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4651ae91c1ab8af36a2800b9b5eb3cb08c5a13cf19fe563aae1fc1d13be8833`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 739.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18665cd1d0000877ad3ef689d96d10bb43c098dff34717b0e17ac9d04ef5ace`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4c94998c413cc533560b47d6afac69ebdc6037cff2dabf530a90135d980ede`  
		Last Modified: Wed, 01 Feb 2023 18:20:43 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d3f1cbafefcfd0a5136a2f172055fb2c456d491320719ae320e3e8e71771bd`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28f154ea67856aa73cfde3cd5bacfa7b5821994cc62f7aa9c393b19c2eeafbf`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:0da3172d19deeb8eb825ed8a84c407710833f767f0778f048b08e7a460e58bf4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:27442f3b0200d77b37168f5687f30e2a999947ef0a5db598c4750e97fb92e3d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **600.3 MB (600285393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5ec1dd33ec9082d8c2d7e9a150579b5193c1f6d18df628b4decf3bec9209055`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:25:04 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:25:04 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:25:04 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:25:27 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:25:28 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3
# Wed, 01 Feb 2023 18:25:28 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb
# Wed, 01 Feb 2023 18:25:28 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:25:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:25:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:26:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=bdc1ffbd5a0eca07a554856a92eb0b5930b457c1d13fca9a2a93ef91a5d88156            ;;          'amd64')            CB_SHA256=bd8c808771cb46e563c173f60e0723c32351a6453f6ece2d4fa440e0d2dcdfd3            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:26:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:26:31 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:26:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:26:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:26:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:26:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:26:33 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:26:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:26:33 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:26:33 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:26:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b4cf586c4b7a57fc5e73b3aa283d12081f9bd7606b6b60d897f2783e6efa0d`  
		Last Modified: Wed, 01 Feb 2023 18:31:06 GMT  
		Size: 6.2 MB (6216449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2820c7121f0a09d4a6b11881f09b95cacc3cbebc82f73aff1f996202193ce0`  
		Last Modified: Wed, 01 Feb 2023 18:31:05 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db5dca17b86b88c0c7cf2b23d43c1ed0561f66106e0b0a955667da1dc1401`  
		Last Modified: Wed, 01 Feb 2023 18:32:01 GMT  
		Size: 565.5 MB (565486707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d11bb0b33cc4ea595033a41004eeea233f267374a44a5dc97bd226bcb64e0d8`  
		Last Modified: Wed, 01 Feb 2023 18:31:05 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a801c20d9d04c9fffd9c9584e4383bf75463ec98280eb032175223dfb87f1980`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 739.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2988e82038abb9d711b27510974291e14223e2834c95c920ce5938a6e7a2c2c`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35420a0cd22388f3cc77425bfc3f5d128433747095ebac6d391c01742be295c`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bea392911ee85dcff4c4d9224495188208fa48c7c4022a52c08b7788dad184`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe9dae4957e5be3f0645755f477cb900b50908d1d7587c4ff46ab294f41d8e4`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:enterprise` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:3c4cabfcbeead72e9ce88f6051d46a67adeeb7b6c16799531b60712cb35c3a4b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.4 MB (574395108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5d8125b01452ee161b3c515386eb7ed92cafd6950fe5e0fad033a50d4dd2b7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:17:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:17:34 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:17:34 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:17:53 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:17:54 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3
# Wed, 01 Feb 2023 18:17:54 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb
# Wed, 01 Feb 2023 18:17:54 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:17:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:17:54 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:18:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=bdc1ffbd5a0eca07a554856a92eb0b5930b457c1d13fca9a2a93ef91a5d88156            ;;          'amd64')            CB_SHA256=bd8c808771cb46e563c173f60e0723c32351a6453f6ece2d4fa440e0d2dcdfd3            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:18:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:18:46 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:18:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:18:47 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:18:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:18:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:18:48 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:18:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:18:48 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:18:48 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:18:48 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df4acc3280127d63542436253f90f4862c9daaef8ed9ea6e07468221a331164`  
		Last Modified: Wed, 01 Feb 2023 18:19:49 GMT  
		Size: 6.0 MB (6039600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56507591370d4d0a4f9266f6983fc882e469e4c9e18638607ebcd310f752bee`  
		Last Modified: Wed, 01 Feb 2023 18:19:48 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e665174c1121b08e9cbfe29177246dd777f3e9f7f7222abbda480985d136c9`  
		Last Modified: Wed, 01 Feb 2023 18:20:29 GMT  
		Size: 541.2 MB (541157405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed85a620835a4af7f402e88ce29f4abe542cb789ee87df6ac7513ae079e815b`  
		Last Modified: Wed, 01 Feb 2023 18:19:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a08982e57dc712bd074870be2d27ccac43380110e21f0a57ea08ee47e34eaf2`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8faa6408783f533b1322b793f5af9800d0ec262eb2fa039646f2587c969500f`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9cd106ccd30da4072a96b97d251a59e8fb9fdf30cf9ad2b3a7910759145851`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2337915ae138787ede0fb08dca68b24dcb59dc626bdda5fe902b142896f7919a`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11379d1c166bf612fc0e058e00faa700dcae528cbff06925c1fe5394db7f0b46`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.6`

```console
$ docker pull couchbase@sha256:6f81f5e905693699c40d748fc87a55b33373f7707f34ba62a4081b89c4ff9c8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.6` - linux; amd64

```console
$ docker pull couchbase@sha256:732324fc9d9f651f81b9f71a856a7626ab1dd8a43d125082cb9661e657dc2cf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.9 MB (531947740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cb9fb9b73bc5e125f3c752235b67f567c89cd23ba831d1f04a463bc7db37233`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:25:04 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:25:04 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:25:04 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:25:27 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:29:49 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6
# Wed, 01 Feb 2023 18:29:49 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb
# Wed, 01 Feb 2023 18:29:49 GMT
ARG CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa
# Wed, 01 Feb 2023 18:29:49 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:29:49 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Wed, 01 Feb 2023 18:29:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:29:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:30:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:30:42 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:30:42 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:30:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:30:43 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:30:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:30:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:30:44 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:30:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:30:44 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:30:44 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:30:44 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b4cf586c4b7a57fc5e73b3aa283d12081f9bd7606b6b60d897f2783e6efa0d`  
		Last Modified: Wed, 01 Feb 2023 18:31:06 GMT  
		Size: 6.2 MB (6216449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5740863927d97994ec3d21c6de0af467b0ae510d8b0293c8e74c73ec07f5ae0`  
		Last Modified: Wed, 01 Feb 2023 18:35:13 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d164b95c54f4b3fdd0d6e30b6d600d3915718d54a8bf5253c84358ef7c72a5`  
		Last Modified: Wed, 01 Feb 2023 18:36:03 GMT  
		Size: 497.1 MB (497149037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c584dbdd2a7bd3addb8f233ef50d596406de06899eee48d88dcd761f842a320`  
		Last Modified: Wed, 01 Feb 2023 18:35:13 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8fa8bc7de4e50e414cb9a0484780220be102116142d15bfb0224867be0d6a1`  
		Last Modified: Wed, 01 Feb 2023 18:35:11 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0bc4a117c18c99798b1f51f2240a6ce57140c30f471c903b58f1adf772b0b8`  
		Last Modified: Wed, 01 Feb 2023 18:35:11 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e70f25ba12d1bcccb97dad4d9b8a50645d0b1a8ef7bcb0247abb2232e5634a`  
		Last Modified: Wed, 01 Feb 2023 18:35:11 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ec254ae18d152e1db206ddc4668eae893cc6dae5b8cbea0f8e2dba7e52328c`  
		Last Modified: Wed, 01 Feb 2023 18:35:11 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cfb26fc8248bff887d3cde118fa5b5c41d9cb9904b7710823c1b7c1a5f947`  
		Last Modified: Wed, 01 Feb 2023 18:35:11 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.0.5`

```console
$ docker pull couchbase@sha256:70d1600c289c834e69caaea2c8c981b5a9ebc245e91d6d729bd333e77f95c072
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:afa70468149f42aa257d2fdc35c6b4d748dfe077abd7f101a040ec5080b119d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **616.6 MB (616628710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c670efa3cc51d5c7a1ae1bef657131d726a397c150d225219e0593613b5dc0e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:25:04 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:25:04 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:25:04 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:25:27 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:27:30 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5
# Wed, 01 Feb 2023 18:27:30 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb
# Wed, 01 Feb 2023 18:27:31 GMT
ARG CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea
# Wed, 01 Feb 2023 18:27:31 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:27:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:27:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:28:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:28:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:28:31 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:28:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:28:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:28:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:28:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:28:33 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:28:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:28:33 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:28:33 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:28:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b4cf586c4b7a57fc5e73b3aa283d12081f9bd7606b6b60d897f2783e6efa0d`  
		Last Modified: Wed, 01 Feb 2023 18:31:06 GMT  
		Size: 6.2 MB (6216449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507b7a7e538510c11f6158504c6a0cc9e16b8dd599ac2f8515b103b246de8e21`  
		Last Modified: Wed, 01 Feb 2023 18:33:05 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de73b439ff8a91b36710c23edc8ca56c4e921ef41b2e6cb71224ea3b546b3aa`  
		Last Modified: Wed, 01 Feb 2023 18:34:03 GMT  
		Size: 581.8 MB (581830013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0738cfd3ccb6b0abfd4708b88a453af4c05a739ed6058036452db84dd98c54`  
		Last Modified: Wed, 01 Feb 2023 18:33:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81320e19b263a40ecbae84dfcba6bd77c9d19dcb14dc1b9633db54316234e955`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 741.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5e61bf65fb7021f8f7fd08cc267e9e3d2bab7e16ead1a46300ae4fa8bd4fe0`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d065117ea502454506cbd8e4c642c1a45641130b86465e564daa4dade7b495a`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ef5abe6b3270b049506d26a9c2b97d6470bdd23f5004da355c317a9e076005`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85caa0ee6487d6e3f055aa6ccb1420be7f7e05020ab26456a63a9fe63b655b62`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.1.3`

```console
$ docker pull couchbase@sha256:0da3172d19deeb8eb825ed8a84c407710833f767f0778f048b08e7a460e58bf4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise-7.1.3` - linux; amd64

```console
$ docker pull couchbase@sha256:27442f3b0200d77b37168f5687f30e2a999947ef0a5db598c4750e97fb92e3d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **600.3 MB (600285393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5ec1dd33ec9082d8c2d7e9a150579b5193c1f6d18df628b4decf3bec9209055`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:25:04 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:25:04 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:25:04 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:25:27 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:25:28 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3
# Wed, 01 Feb 2023 18:25:28 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb
# Wed, 01 Feb 2023 18:25:28 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:25:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:25:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:26:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=bdc1ffbd5a0eca07a554856a92eb0b5930b457c1d13fca9a2a93ef91a5d88156            ;;          'amd64')            CB_SHA256=bd8c808771cb46e563c173f60e0723c32351a6453f6ece2d4fa440e0d2dcdfd3            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:26:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:26:31 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:26:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:26:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:26:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:26:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:26:33 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:26:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:26:33 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:26:33 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:26:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b4cf586c4b7a57fc5e73b3aa283d12081f9bd7606b6b60d897f2783e6efa0d`  
		Last Modified: Wed, 01 Feb 2023 18:31:06 GMT  
		Size: 6.2 MB (6216449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2820c7121f0a09d4a6b11881f09b95cacc3cbebc82f73aff1f996202193ce0`  
		Last Modified: Wed, 01 Feb 2023 18:31:05 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db5dca17b86b88c0c7cf2b23d43c1ed0561f66106e0b0a955667da1dc1401`  
		Last Modified: Wed, 01 Feb 2023 18:32:01 GMT  
		Size: 565.5 MB (565486707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d11bb0b33cc4ea595033a41004eeea233f267374a44a5dc97bd226bcb64e0d8`  
		Last Modified: Wed, 01 Feb 2023 18:31:05 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a801c20d9d04c9fffd9c9584e4383bf75463ec98280eb032175223dfb87f1980`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 739.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2988e82038abb9d711b27510974291e14223e2834c95c920ce5938a6e7a2c2c`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35420a0cd22388f3cc77425bfc3f5d128433747095ebac6d391c01742be295c`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bea392911ee85dcff4c4d9224495188208fa48c7c4022a52c08b7788dad184`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe9dae4957e5be3f0645755f477cb900b50908d1d7587c4ff46ab294f41d8e4`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:enterprise-7.1.3` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:3c4cabfcbeead72e9ce88f6051d46a67adeeb7b6c16799531b60712cb35c3a4b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.4 MB (574395108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5d8125b01452ee161b3c515386eb7ed92cafd6950fe5e0fad033a50d4dd2b7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:17:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:17:34 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:17:34 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:17:53 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:17:54 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3
# Wed, 01 Feb 2023 18:17:54 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb
# Wed, 01 Feb 2023 18:17:54 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:17:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:17:54 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:18:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=bdc1ffbd5a0eca07a554856a92eb0b5930b457c1d13fca9a2a93ef91a5d88156            ;;          'amd64')            CB_SHA256=bd8c808771cb46e563c173f60e0723c32351a6453f6ece2d4fa440e0d2dcdfd3            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:18:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:18:46 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:18:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:18:47 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:18:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:18:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:18:48 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:18:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:18:48 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:18:48 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:18:48 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df4acc3280127d63542436253f90f4862c9daaef8ed9ea6e07468221a331164`  
		Last Modified: Wed, 01 Feb 2023 18:19:49 GMT  
		Size: 6.0 MB (6039600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56507591370d4d0a4f9266f6983fc882e469e4c9e18638607ebcd310f752bee`  
		Last Modified: Wed, 01 Feb 2023 18:19:48 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e665174c1121b08e9cbfe29177246dd777f3e9f7f7222abbda480985d136c9`  
		Last Modified: Wed, 01 Feb 2023 18:20:29 GMT  
		Size: 541.2 MB (541157405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed85a620835a4af7f402e88ce29f4abe542cb789ee87df6ac7513ae079e815b`  
		Last Modified: Wed, 01 Feb 2023 18:19:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a08982e57dc712bd074870be2d27ccac43380110e21f0a57ea08ee47e34eaf2`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8faa6408783f533b1322b793f5af9800d0ec262eb2fa039646f2587c969500f`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9cd106ccd30da4072a96b97d251a59e8fb9fdf30cf9ad2b3a7910759145851`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2337915ae138787ede0fb08dca68b24dcb59dc626bdda5fe902b142896f7919a`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11379d1c166bf612fc0e058e00faa700dcae528cbff06925c1fe5394db7f0b46`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:0da3172d19deeb8eb825ed8a84c407710833f767f0778f048b08e7a460e58bf4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:27442f3b0200d77b37168f5687f30e2a999947ef0a5db598c4750e97fb92e3d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **600.3 MB (600285393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5ec1dd33ec9082d8c2d7e9a150579b5193c1f6d18df628b4decf3bec9209055`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:25:04 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:25:04 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:25:04 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:25:27 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:25:28 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3
# Wed, 01 Feb 2023 18:25:28 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb
# Wed, 01 Feb 2023 18:25:28 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:25:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:25:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:26:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=bdc1ffbd5a0eca07a554856a92eb0b5930b457c1d13fca9a2a93ef91a5d88156            ;;          'amd64')            CB_SHA256=bd8c808771cb46e563c173f60e0723c32351a6453f6ece2d4fa440e0d2dcdfd3            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:26:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:26:31 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:26:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:26:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:26:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:26:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:26:33 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:26:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:26:33 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:26:33 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:26:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b4cf586c4b7a57fc5e73b3aa283d12081f9bd7606b6b60d897f2783e6efa0d`  
		Last Modified: Wed, 01 Feb 2023 18:31:06 GMT  
		Size: 6.2 MB (6216449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2820c7121f0a09d4a6b11881f09b95cacc3cbebc82f73aff1f996202193ce0`  
		Last Modified: Wed, 01 Feb 2023 18:31:05 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db5dca17b86b88c0c7cf2b23d43c1ed0561f66106e0b0a955667da1dc1401`  
		Last Modified: Wed, 01 Feb 2023 18:32:01 GMT  
		Size: 565.5 MB (565486707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d11bb0b33cc4ea595033a41004eeea233f267374a44a5dc97bd226bcb64e0d8`  
		Last Modified: Wed, 01 Feb 2023 18:31:05 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a801c20d9d04c9fffd9c9584e4383bf75463ec98280eb032175223dfb87f1980`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 739.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2988e82038abb9d711b27510974291e14223e2834c95c920ce5938a6e7a2c2c`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35420a0cd22388f3cc77425bfc3f5d128433747095ebac6d391c01742be295c`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bea392911ee85dcff4c4d9224495188208fa48c7c4022a52c08b7788dad184`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe9dae4957e5be3f0645755f477cb900b50908d1d7587c4ff46ab294f41d8e4`  
		Last Modified: Wed, 01 Feb 2023 18:31:03 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:latest` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:3c4cabfcbeead72e9ce88f6051d46a67adeeb7b6c16799531b60712cb35c3a4b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.4 MB (574395108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5d8125b01452ee161b3c515386eb7ed92cafd6950fe5e0fad033a50d4dd2b7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:17:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:17:34 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:17:34 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:17:53 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:17:54 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3
# Wed, 01 Feb 2023 18:17:54 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb
# Wed, 01 Feb 2023 18:17:54 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:17:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:17:54 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:18:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=bdc1ffbd5a0eca07a554856a92eb0b5930b457c1d13fca9a2a93ef91a5d88156            ;;          'amd64')            CB_SHA256=bd8c808771cb46e563c173f60e0723c32351a6453f6ece2d4fa440e0d2dcdfd3            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:18:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:18:46 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:18:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:18:47 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:18:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:18:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.3-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.3 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:18:48 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:18:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:18:48 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:18:48 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:18:48 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df4acc3280127d63542436253f90f4862c9daaef8ed9ea6e07468221a331164`  
		Last Modified: Wed, 01 Feb 2023 18:19:49 GMT  
		Size: 6.0 MB (6039600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56507591370d4d0a4f9266f6983fc882e469e4c9e18638607ebcd310f752bee`  
		Last Modified: Wed, 01 Feb 2023 18:19:48 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e665174c1121b08e9cbfe29177246dd777f3e9f7f7222abbda480985d136c9`  
		Last Modified: Wed, 01 Feb 2023 18:20:29 GMT  
		Size: 541.2 MB (541157405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed85a620835a4af7f402e88ce29f4abe542cb789ee87df6ac7513ae079e815b`  
		Last Modified: Wed, 01 Feb 2023 18:19:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a08982e57dc712bd074870be2d27ccac43380110e21f0a57ea08ee47e34eaf2`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8faa6408783f533b1322b793f5af9800d0ec262eb2fa039646f2587c969500f`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9cd106ccd30da4072a96b97d251a59e8fb9fdf30cf9ad2b3a7910759145851`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2337915ae138787ede0fb08dca68b24dcb59dc626bdda5fe902b142896f7919a`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11379d1c166bf612fc0e058e00faa700dcae528cbff06925c1fe5394db7f0b46`  
		Last Modified: Wed, 01 Feb 2023 18:19:46 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
