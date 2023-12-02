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
