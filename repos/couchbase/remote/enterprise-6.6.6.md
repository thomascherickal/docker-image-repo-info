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
