<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchbase`

-	[`couchbase:6.6.6`](#couchbase666)
-	[`couchbase:7.0.5`](#couchbase705)
-	[`couchbase:7.1.5`](#couchbase715)
-	[`couchbase:7.2.1`](#couchbase721)
-	[`couchbase:community`](#couchbasecommunity)
-	[`couchbase:community-6.6.0`](#couchbasecommunity-660)
-	[`couchbase:community-7.0.2`](#couchbasecommunity-702)
-	[`couchbase:community-7.1.1`](#couchbasecommunity-711)
-	[`couchbase:community-7.2.1`](#couchbasecommunity-721)
-	[`couchbase:enterprise`](#couchbaseenterprise)
-	[`couchbase:enterprise-6.6.6`](#couchbaseenterprise-666)
-	[`couchbase:enterprise-7.0.5`](#couchbaseenterprise-705)
-	[`couchbase:enterprise-7.1.5`](#couchbaseenterprise-715)
-	[`couchbase:enterprise-7.2.1`](#couchbaseenterprise-721)
-	[`couchbase:latest`](#couchbaselatest)

## `couchbase:6.6.6`

```console
$ docker pull couchbase@sha256:b1a23eddd21a1d3bcf03fecc66f9f2595cdade8553911f37c08c59c08e830338
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.6` - linux; amd64

```console
$ docker pull couchbase@sha256:0a16bda78c3e9606ea2cc88f614493abc653e5da5e062c9c4f285712aae85856
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.0 MB (532019586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589bca18245972f4357be12cb94952b66ce0f1aa62e7dc4aa36db6e85af56644`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:54:54 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 02:54:54 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 02:54:54 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:55:09 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 03 Aug 2023 03:02:18 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6
# Thu, 03 Aug 2023 03:02:18 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb
# Thu, 03 Aug 2023 03:02:18 GMT
ARG CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa
# Thu, 03 Aug 2023 03:02:18 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 03 Aug 2023 03:02:18 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Thu, 03 Aug 2023 03:02:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 03:02:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 03:03:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 03:03:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 03:03:17 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 03:03:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 03:03:18 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:03:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 03:03:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 03 Aug 2023 03:03:19 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 03 Aug 2023 03:03:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 03:03:19 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 03:03:19 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Thu, 03 Aug 2023 03:03:19 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35618df5c9a71269b91577e6aea59155f8edb63501d542ce129979a4d9e328b`  
		Last Modified: Thu, 03 Aug 2023 03:03:49 GMT  
		Size: 6.3 MB (6285930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b3a69a5ad6f03a3f4a445bb2ee9c4b3eae6877f28386015cdfb95c686ca66a`  
		Last Modified: Thu, 03 Aug 2023 03:09:36 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a3e1cb73494f1b9a9da4eba5b1aacfab98db03861d518050814ff6b765384d`  
		Last Modified: Thu, 03 Aug 2023 03:10:20 GMT  
		Size: 497.1 MB (497148623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479a1455825b1e7f46b1f4e3a4f38be68bafaf261c3e966d0b5ece48f30f6a49`  
		Last Modified: Thu, 03 Aug 2023 03:09:36 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa139d04f2ae93d8a126e07633c875b79ea2b8bf98b5ad4a18eb70788109a11`  
		Last Modified: Thu, 03 Aug 2023 03:09:34 GMT  
		Size: 741.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25bc5d9275e08030f28b782d2368a5e3252a5cc6df8c00b530368815c849ba4`  
		Last Modified: Thu, 03 Aug 2023 03:09:35 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3396770093741a604eba6cf3c036039d18e18decae891394cea9780554b0207`  
		Last Modified: Thu, 03 Aug 2023 03:09:34 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11cf9530ca1bdcc8cd1110f975a3abcb9bd2d7689285c9088c2076679f4268e`  
		Last Modified: Thu, 03 Aug 2023 03:09:34 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69688afb0eadca8780963a6a44f6c69899da47010a3627f58dfad0bfbc72dc41`  
		Last Modified: Thu, 03 Aug 2023 03:09:34 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.0.5`

```console
$ docker pull couchbase@sha256:80147874189584c6c23fe09f86bcd02fdd4c68c152e367c89ce929e4c0b35989
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:7.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:021ca5807cb24b470c37b2e24f1927e86ab1118c039ab2b99007df983518debc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **616.7 MB (616700977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7beebceb98d2f7b7f01b7cc186b6f63a4c24c64ca51257575cfb43e63b7d33e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:54:54 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 02:54:54 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 02:54:54 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:55:09 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 03 Aug 2023 02:59:44 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5
# Thu, 03 Aug 2023 02:59:44 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb
# Thu, 03 Aug 2023 02:59:44 GMT
ARG CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea
# Thu, 03 Aug 2023 02:59:44 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 03 Aug 2023 02:59:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 02:59:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 03:00:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 03:00:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 03:00:52 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 03:00:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 03:00:53 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:00:53 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 03:00:53 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 03 Aug 2023 03:00:54 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 03 Aug 2023 03:00:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 03:00:54 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 03:00:54 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Thu, 03 Aug 2023 03:00:54 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35618df5c9a71269b91577e6aea59155f8edb63501d542ce129979a4d9e328b`  
		Last Modified: Thu, 03 Aug 2023 03:03:49 GMT  
		Size: 6.3 MB (6285930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f23d74a607dd246cb492e41911e0870aa54ce28bc02c98bee7647b0d719301`  
		Last Modified: Thu, 03 Aug 2023 03:07:39 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c02a2d7ad3410f14faf3e87475bb895cc4c735b9e906cb4ee8eece2c43306a`  
		Last Modified: Thu, 03 Aug 2023 03:08:32 GMT  
		Size: 581.8 MB (581830015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd83a76ab988da2237ecc5fb4cdfe8ac30189561e9cfe1fe52a75d0eef7b42cd`  
		Last Modified: Thu, 03 Aug 2023 03:07:39 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413e65edcbdb6f1db1a64c63017c72cb8a5cb4908bcb27875fa45614f7d7e4cd`  
		Last Modified: Thu, 03 Aug 2023 03:07:37 GMT  
		Size: 739.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63b275fb5763131fb757c3fbb603610ea72dc5124b50d40b17035e42b9874bd`  
		Last Modified: Thu, 03 Aug 2023 03:07:37 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd561df3edd02685f9cb39a9b23b7b14c445fed30a6ba42cc398bc7403709c6`  
		Last Modified: Thu, 03 Aug 2023 03:07:37 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d54f51e85ea641e2ad600dfd0b24a55cea21cd042c7bff56117db7e2cc6ab`  
		Last Modified: Thu, 03 Aug 2023 03:07:37 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455d32fa519253eb3b01b31803fe2b627f33be0339edf1df99834c84d52a3aba`  
		Last Modified: Thu, 03 Aug 2023 03:07:37 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.1.5`

```console
$ docker pull couchbase@sha256:d27a35f7be9298397cd7f270f6b655ff10b647bf283a1b87a09291cc951e9922
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:7.1.5` - linux; amd64

```console
$ docker pull couchbase@sha256:d79a10ae6216fbc9f695c2168b94b7a8a73a15cbf1988176be68405c90c8d198
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **643.4 MB (643404561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acfb11ee5affaa83a7b8bcf7419bd3312f9f9692e62e38296de777413b526be8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:54:54 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 02:54:54 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 02:54:54 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:55:09 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Fri, 04 Aug 2023 00:24:36 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5
# Fri, 04 Aug 2023 00:24:37 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb
# Fri, 04 Aug 2023 00:24:37 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 04 Aug 2023 00:24:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 04 Aug 2023 00:24:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 04 Aug 2023 00:25:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=57ecac55aca0abf1e6f0a62ebdcd24514cf0d87d09498d794b047d533719321a            ;;          'amd64')            CB_SHA256=b4e3a4f7d10b34471a7ba8a03ac658e79778aaf6b091c9c1631a5c4548e102e0            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 04 Aug 2023 00:26:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 04 Aug 2023 00:26:01 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 04 Aug 2023 00:26:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 04 Aug 2023 00:26:02 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 04 Aug 2023 00:26:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 04 Aug 2023 00:26:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 04 Aug 2023 00:26:03 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 04 Aug 2023 00:26:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 04 Aug 2023 00:26:03 GMT
CMD ["couchbase-server"]
# Fri, 04 Aug 2023 00:26:03 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 04 Aug 2023 00:26:03 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35618df5c9a71269b91577e6aea59155f8edb63501d542ce129979a4d9e328b`  
		Last Modified: Thu, 03 Aug 2023 03:03:49 GMT  
		Size: 6.3 MB (6285930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1257a92c9cfb195b5dd450984903a49323dfdc2dfc6a93b28bf017d96da1f62`  
		Last Modified: Fri, 04 Aug 2023 00:26:45 GMT  
		Size: 1.8 KB (1832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f896d6db571df7b05bc58895c4f7eb33357a50e7fd42c82552a5a1b279418a1`  
		Last Modified: Fri, 04 Aug 2023 00:27:39 GMT  
		Size: 608.5 MB (608533596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc1a46db1570a7eab075a4fb15e83ea5953b875947e533c28aa6cac04ac5dc0`  
		Last Modified: Fri, 04 Aug 2023 00:26:45 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da881006ba56a8bba8cab5eabd4d5f75d5da870b55bb6d543b8f914f742c48b0`  
		Last Modified: Fri, 04 Aug 2023 00:26:43 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8670f2149e78c0e3011851211122aaea50e4429c2847b3c1cc8492aa157743c1`  
		Last Modified: Fri, 04 Aug 2023 00:26:43 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99d460e99a3ec9b231bce484f3c5cb00a0db3a74c3a88df0772a76398353013`  
		Last Modified: Fri, 04 Aug 2023 00:26:43 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a36d7a79c35149244f4ebc6b4305f358151715777ecd04f6da1594334fe7316`  
		Last Modified: Fri, 04 Aug 2023 00:26:46 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d74e13a3f853590260bd93f413041f81b384be15a100bd67f09238350db84c7`  
		Last Modified: Fri, 04 Aug 2023 00:26:43 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:7.1.5` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:ea591345fa7ed81a45b3f36a8227db3f6d753df3931ec3436916c2505c259000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.6 MB (617567819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:506076be4a8c2b004cd0406167c2fd1151db359a9dc886dba92784012f94dc68`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:13:43 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 01:13:43 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 01:13:43 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 01:14:01 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Fri, 04 Aug 2023 00:53:42 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5
# Fri, 04 Aug 2023 00:53:42 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb
# Fri, 04 Aug 2023 00:53:42 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 04 Aug 2023 00:53:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 04 Aug 2023 00:53:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 04 Aug 2023 00:54:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=57ecac55aca0abf1e6f0a62ebdcd24514cf0d87d09498d794b047d533719321a            ;;          'amd64')            CB_SHA256=b4e3a4f7d10b34471a7ba8a03ac658e79778aaf6b091c9c1631a5c4548e102e0            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 04 Aug 2023 00:54:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 04 Aug 2023 00:54:47 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 04 Aug 2023 00:54:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 04 Aug 2023 00:54:48 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 04 Aug 2023 00:54:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 04 Aug 2023 00:54:49 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 04 Aug 2023 00:54:49 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 04 Aug 2023 00:54:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 04 Aug 2023 00:54:49 GMT
CMD ["couchbase-server"]
# Fri, 04 Aug 2023 00:54:49 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 04 Aug 2023 00:54:49 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad91e7dfaee3352f726a7133ee4af8e38e1f989f4a537f0618abd00bb4c784e`  
		Last Modified: Thu, 03 Aug 2023 01:18:32 GMT  
		Size: 6.1 MB (6110566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f21b205b426f8b3797298acb8e8a75ac504273872cd7921181e3ba9e9b9aae8`  
		Last Modified: Fri, 04 Aug 2023 00:55:08 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e28d875d834a20ae5495b7ce03dd1e973a6ef018ebad30c2ae4c564946a31d7`  
		Last Modified: Fri, 04 Aug 2023 00:55:50 GMT  
		Size: 584.3 MB (584252302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3c5c9949e75bf9cd61a65b90d82b46799541cce82143e9bfad5481e62e5486`  
		Last Modified: Fri, 04 Aug 2023 00:55:07 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ab53f93402b9f9d6d5164cafb4cd163f0aa5a8783e8a1e9472160d95bf1fc6`  
		Last Modified: Fri, 04 Aug 2023 00:55:06 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39ee9d005c164ede9fb4b9ad30b287dea61025cc5a6cfb825543e423d17bb33`  
		Last Modified: Fri, 04 Aug 2023 00:55:06 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49fce06a7532519eb2827348dcd266bb968cf19274cf22ac49682f1a46649cd`  
		Last Modified: Fri, 04 Aug 2023 00:55:06 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2c9c5f9bf13ba8153a3b6af6e17cddd2871cd4fc518972516ca13f899b8081`  
		Last Modified: Fri, 04 Aug 2023 00:55:06 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9cec6241af27697a9d9c1caa0e55ecec8da6eb3324d8500ba5b4bba1a63744`  
		Last Modified: Fri, 04 Aug 2023 00:55:06 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.2.1`

```console
$ docker pull couchbase@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `couchbase:community`

```console
$ docker pull couchbase@sha256:580ef32893ec74eb070d59f0e267bf9069ffadaaccd175a09a650f275e3e8f55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:d581a356ec8e5a4edd58086fcfff60c3bcbf57f629dc3cb3e92ccc17537ebf80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357144300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f69d43f1cb82c428ca8a164618cb9e0dd9dc0c3eb67d8a7047b5fe4488a8090`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:54:54 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 02:54:54 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 02:54:54 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:55:09 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 03 Aug 2023 02:55:10 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0
# Thu, 03 Aug 2023 02:56:33 GMT
ARG CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb
# Thu, 03 Aug 2023 02:56:33 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 03 Aug 2023 02:56:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 02:56:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 02:57:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=0877ec5c4109992fc2186ecf6153d7f30a24be7f6559133c855ecff77b9b2363            ;;          'amd64')            CB_SHA256=6c07122d9e28c0679c012cba73c28df76a74424cf206fedf42c7e18fa640b6b1            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:57:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 02:57:17 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 02:57:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 02:57:18 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 02:57:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 02:57:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 03 Aug 2023 02:57:19 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 03 Aug 2023 02:57:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 02:57:19 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 02:57:19 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Thu, 03 Aug 2023 02:57:19 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35618df5c9a71269b91577e6aea59155f8edb63501d542ce129979a4d9e328b`  
		Last Modified: Thu, 03 Aug 2023 03:03:49 GMT  
		Size: 6.3 MB (6285930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9e41c93bd38e3d7fdf86eadfe0151f9734ceff7e79a5a6145bcd35f946ae28`  
		Last Modified: Thu, 03 Aug 2023 03:05:01 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5632644e8d86888dbc0c089ef9a799b763decf6608e7dcbe3bed9799557579ac`  
		Last Modified: Thu, 03 Aug 2023 03:05:37 GMT  
		Size: 322.3 MB (322273343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4602f313633c16d97e25528f307259b5e8f021aed28d78fadc1fdb06be7a7057`  
		Last Modified: Thu, 03 Aug 2023 03:05:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1717e0b83c6b95798f94427c6e9bf582eaaa8162d027849f4675e20b7dd666e1`  
		Last Modified: Thu, 03 Aug 2023 03:04:59 GMT  
		Size: 738.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651857319e9313aaa090d5a37fa79092c6c6d6461a31ba2d732eb3a23946681b`  
		Last Modified: Thu, 03 Aug 2023 03:04:59 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56226190e7500bbbcd87a52b1b4e832f0f16ddcd23445515d1ec9fe0ad2d3452`  
		Last Modified: Thu, 03 Aug 2023 03:04:59 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df454e98a14bbc6d686c397cd8f0a91f0027d67e7823342e372c81d08fc1560f`  
		Last Modified: Thu, 03 Aug 2023 03:04:59 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e9de64bb6b795340dccecdff38f79aa00f6e42552836bb675503ed427b3272`  
		Last Modified: Thu, 03 Aug 2023 03:04:59 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:768fb3231cda398b6037ef94711baf3cbf63e042e255460a324d2f3cfa512316
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.6 MB (335640659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d238841d3f4a0cc6037724bbfff2ccbaf4ff8eaa0b51c09b60fd362b71936077`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:13:43 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 01:13:43 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 01:13:43 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 01:14:01 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 03 Aug 2023 01:14:02 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0
# Thu, 03 Aug 2023 01:15:21 GMT
ARG CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb
# Thu, 03 Aug 2023 01:15:21 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 03 Aug 2023 01:15:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 01:15:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 01:15:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=0877ec5c4109992fc2186ecf6153d7f30a24be7f6559133c855ecff77b9b2363            ;;          'amd64')            CB_SHA256=6c07122d9e28c0679c012cba73c28df76a74424cf206fedf42c7e18fa640b6b1            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 01:16:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 01:16:02 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 01:16:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 01:16:03 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 01:16:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 01:16:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 03 Aug 2023 01:16:04 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 03 Aug 2023 01:16:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 01:16:04 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 01:16:04 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Thu, 03 Aug 2023 01:16:04 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad91e7dfaee3352f726a7133ee4af8e38e1f989f4a537f0618abd00bb4c784e`  
		Last Modified: Thu, 03 Aug 2023 01:18:32 GMT  
		Size: 6.1 MB (6110566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefecead7df3f5aa37a70d9e442ce43ad22c79b54655c79940ea2f69d65bb966`  
		Last Modified: Thu, 03 Aug 2023 01:19:30 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc1584daf4c996a64d74df8ed87fcc8e727950c3418a5986323ef83ad48bf1c`  
		Last Modified: Thu, 03 Aug 2023 01:19:58 GMT  
		Size: 302.3 MB (302325147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35ac731662e27039bf03d8847fec34e4e2b4f3c62194c0611961fa00780413`  
		Last Modified: Thu, 03 Aug 2023 01:19:30 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e908fc65253bcbf3d19eb2d9ebf53b2a914b27175b4e37ee8e22c78c75d77990`  
		Last Modified: Thu, 03 Aug 2023 01:19:28 GMT  
		Size: 738.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111e60bd32f1d333e21bab75e6996d2da9892b0d2ab926fd5d3c09ec4a8f2eb1`  
		Last Modified: Thu, 03 Aug 2023 01:19:28 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179c85844312c438aa86f9adbfed86fdf551537dae841c3d6f111d881cf2d03c`  
		Last Modified: Thu, 03 Aug 2023 01:19:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f552fc9f0b9bb5b50a7e0458e44a9c9f31b57468a1ac1fb634923a74964cc1fb`  
		Last Modified: Thu, 03 Aug 2023 01:19:29 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93fa8bb145c1ea2655271e27a35fbe2897a1db63a9f0ae20e169c93682689cf`  
		Last Modified: Thu, 03 Aug 2023 01:19:28 GMT  
		Size: 868.0 B  
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
$ docker pull couchbase@sha256:617ee6ff55a214296c299ce95e4526a4d74ecaf48b499228fa5273674c6e39e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.2` - linux; amd64

```console
$ docker pull couchbase@sha256:6a833c452ba826f1e10ada1ef2989b3d522d7e8d34177e302954da9d8a81cf35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.1 MB (429069595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31dc3004e9e9dd2578026abd7dc80cf81c1ba6d462f7e97bcfe77ba39eed4f10`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:54:54 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 03:01:17 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 03:01:18 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Thu, 03 Aug 2023 03:01:18 GMT
ARG CB_VERSION=7.0.2
# Thu, 03 Aug 2023 03:01:18 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Thu, 03 Aug 2023 03:01:18 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb
# Thu, 03 Aug 2023 03:01:18 GMT
ARG CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e
# Thu, 03 Aug 2023 03:01:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 03:01:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 03:01:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 03:02:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 03:02:02 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 03:02:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 03:02:03 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:02:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 03:02:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Thu, 03 Aug 2023 03:02:04 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Thu, 03 Aug 2023 03:02:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 03:02:04 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 03:02:04 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Thu, 03 Aug 2023 03:02:04 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e13408ec75039ce8e11c976848d6f325fc65cf5741238eabc06dda2be96cf3`  
		Last Modified: Thu, 03 Aug 2023 03:08:46 GMT  
		Size: 6.3 MB (6292515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6c7f601ce9a002cfadbc762267bf59ac32971575acc047f1deeea2c87c3a58`  
		Last Modified: Thu, 03 Aug 2023 03:08:43 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9f10d13e2b53192db271ad77cc882ec1468fa3db1d1f683eb9266478d5a835`  
		Last Modified: Thu, 03 Aug 2023 03:08:43 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf04ce8ec9775e458368b40f1eb8633a5a3a3027081bef26ad46996afa78006`  
		Last Modified: Thu, 03 Aug 2023 03:09:27 GMT  
		Size: 394.1 MB (394062421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176313d0d7691d00d880fc06a6637516293bc76864b70b2210459872d634ff09`  
		Last Modified: Thu, 03 Aug 2023 03:08:45 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35ebb3ac025cda259a33705541201644b6bbe26d0e8176326b8584714b12ec6`  
		Last Modified: Thu, 03 Aug 2023 03:08:43 GMT  
		Size: 603.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0297b3e0bc9f5ef29733e3cbc9ade963510e33b386d5f7df700429cd5f17d73`  
		Last Modified: Thu, 03 Aug 2023 03:08:41 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe54d8c9da7939a664ecbc87fed7bcd50c105d0c4fea1acbdff84459983c5577`  
		Last Modified: Thu, 03 Aug 2023 03:08:41 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1c0f5c27c40abedfb3f2fcd486ff32b383047d3d073c9373839d5a92ae11be`  
		Last Modified: Thu, 03 Aug 2023 03:08:41 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1d4dbf511273590ac7b290f6662f7854639ddfe572d4984ae0a0cdad0875d`  
		Last Modified: Thu, 03 Aug 2023 03:08:41 GMT  
		Size: 129.5 KB (129508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dce183ef2f7293459c2d7dd41b589b7fda3e2a226c52ae0c6e4e781b985eaf2`  
		Last Modified: Thu, 03 Aug 2023 03:08:41 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.1.1`

```console
$ docker pull couchbase@sha256:b8203aff69c13980b0ad1e2429830033ec3c47b6cd2776ad25c1c1a687df36df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community-7.1.1` - linux; amd64

```console
$ docker pull couchbase@sha256:e2ec44dbfd3316b986fb7638039fd8c28f098208eabc6c94809d2e303c0ff098
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.7 MB (346670657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cca8288a2f1a49f3e72325a29f37f56fdb0dbe9d1b7e62daca781f2ce4adc29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:54:54 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 02:54:54 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 02:54:54 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:55:09 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 03 Aug 2023 02:58:55 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Thu, 03 Aug 2023 02:58:55 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Thu, 03 Aug 2023 02:58:55 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 03 Aug 2023 02:58:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 02:58:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 02:59:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:59:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 02:59:37 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 02:59:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 02:59:38 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 02:59:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 02:59:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 03 Aug 2023 02:59:39 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 03 Aug 2023 02:59:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 02:59:39 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 02:59:39 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Thu, 03 Aug 2023 02:59:39 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35618df5c9a71269b91577e6aea59155f8edb63501d542ce129979a4d9e328b`  
		Last Modified: Thu, 03 Aug 2023 03:03:49 GMT  
		Size: 6.3 MB (6285930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da9d2bb13bc322a3250afc4e6189734a9974584ebe442221a8211c676027ae6`  
		Last Modified: Thu, 03 Aug 2023 03:06:56 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03a9d0161f1932f4fa8d4ab89a685b3cbdf4157e3b4d75e51188c3068e6e7f7`  
		Last Modified: Thu, 03 Aug 2023 03:07:30 GMT  
		Size: 311.8 MB (311799697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a806e8bd49415b93a9c6f8b73ba65f92594df7740cc905494ed330807c9492`  
		Last Modified: Thu, 03 Aug 2023 03:06:56 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecefe23381cb10cd518bcd4a1b09bf203f9302302e1b238d95d5da9992412aa1`  
		Last Modified: Thu, 03 Aug 2023 03:06:54 GMT  
		Size: 742.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c005a7a0972e7d3579690f84e716994b558e936607aa932f092657c1ab49f1d3`  
		Last Modified: Thu, 03 Aug 2023 03:06:54 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed571114a65d74013a85b49cbf34a511f0b7ad69b9e4a2e16829255868d3ad03`  
		Last Modified: Thu, 03 Aug 2023 03:06:54 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17eceaa93ad500c012d0859308dacede530b4bfdc2be2b53adc74ff63391f3f`  
		Last Modified: Thu, 03 Aug 2023 03:06:54 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e7e3fc26e50ff70d201094067f8206e12cbbb28d166375ca38303766c90097`  
		Last Modified: Thu, 03 Aug 2023 03:06:54 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community-7.1.1` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:5ff7d1b9dfd7bb7d41b19f828895a87b6912efedc2643d543e5ad36daa5542b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.3 MB (327342283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbe3678d31e7bd0b1aaba95b1dbda765948d23b764e020ef28be200f17de51a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:13:43 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 01:13:43 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 01:13:43 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 01:14:01 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 03 Aug 2023 01:17:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Thu, 03 Aug 2023 01:17:32 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Thu, 03 Aug 2023 01:17:32 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 03 Aug 2023 01:17:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 01:17:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 01:18:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 01:18:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 01:18:12 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 01:18:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 01:18:12 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 01:18:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 01:18:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 03 Aug 2023 01:18:13 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 03 Aug 2023 01:18:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 01:18:13 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 01:18:13 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Thu, 03 Aug 2023 01:18:13 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad91e7dfaee3352f726a7133ee4af8e38e1f989f4a537f0618abd00bb4c784e`  
		Last Modified: Thu, 03 Aug 2023 01:18:32 GMT  
		Size: 6.1 MB (6110566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846c3e1a736adb12ae307ac8f3485e5638ca14246d74f1f8c63deec620eabc85`  
		Last Modified: Thu, 03 Aug 2023 01:21:01 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6389d0d5ffc9b8eeefff9cbaf0f5ded7406366ca4eef86db2dbd9d298adc5b`  
		Last Modified: Thu, 03 Aug 2023 01:21:26 GMT  
		Size: 294.0 MB (294026761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5383f2fc61de5844a450e218411bb26a939b4e4f85c2886087cd345a01503f8d`  
		Last Modified: Thu, 03 Aug 2023 01:21:01 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3424eae5b4b5813afb6b5c6604c77e122a507230d2d489a4dc4af3b25eae19ea`  
		Last Modified: Thu, 03 Aug 2023 01:21:00 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd10e6cfe1c5c7bcf2060c35cd8b277bfce39f49365bffe644724deb9fb2e22e`  
		Last Modified: Thu, 03 Aug 2023 01:21:00 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496caa798bdb10158765ee762bdcb6f73b59f6df4a01e7f24bcc930cf7db8e9f`  
		Last Modified: Thu, 03 Aug 2023 01:21:00 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105baf12d4391e4cee6bf2497fe856e134c4e35c48b8fb2e377e0c81f10f6c75`  
		Last Modified: Thu, 03 Aug 2023 01:21:00 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b776c714eefc8eee02f2038cf66eedbdc05345b802c68470ddb23582ab790df3`  
		Last Modified: Thu, 03 Aug 2023 01:21:00 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.2.1`

```console
$ docker pull couchbase@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:76114e559a863fde21c7b327ac82c3b5e265599e259ea8731f3c739c42e65464
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:772a2c8fcc3e4a65e410053e5b4f1a4c5349da0ccb78de4d458cf91e49719263
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **663.7 MB (663685101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232147af3c363497c044401c3a221e39f18ad490a26bf4efc84e5e972db019c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:54:54 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 02:54:54 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 02:54:54 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:55:09 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 03 Aug 2023 02:55:10 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0
# Thu, 03 Aug 2023 02:55:10 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb
# Thu, 03 Aug 2023 02:55:10 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 03 Aug 2023 02:55:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 02:55:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 02:56:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=b44a4d8e577613ad027dbac9830e6123deb7bda22facefe687d6b6e98c86ac66            ;;          'amd64')            CB_SHA256=2fd31b46a6df5ed9c85d3a6cadfb0214e3f928c14ff0b03e6a24652700128328            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:56:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 02:56:26 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 02:56:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 02:56:26 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 02:56:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 02:56:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 03 Aug 2023 02:56:27 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 03 Aug 2023 02:56:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 02:56:28 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 02:56:28 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Thu, 03 Aug 2023 02:56:28 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35618df5c9a71269b91577e6aea59155f8edb63501d542ce129979a4d9e328b`  
		Last Modified: Thu, 03 Aug 2023 03:03:49 GMT  
		Size: 6.3 MB (6285930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76951ffea2eb9305de925d27044022b82719478ca00eb5b6aa7c90bef872ed3a`  
		Last Modified: Thu, 03 Aug 2023 03:03:47 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91aeb93d2aa72ad20c4cf699740572ef7fd37fa590584cbbb57e54731b7b6cad`  
		Last Modified: Thu, 03 Aug 2023 03:04:45 GMT  
		Size: 628.8 MB (628814146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d05cef67ec666d42e81e534724fed4d45134c72ee363e7a29f01a2ce99df6f`  
		Last Modified: Thu, 03 Aug 2023 03:03:47 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f693b82a631465ff6992c15eb0c719a8520cd5aea5e5b792f56780e5198372`  
		Last Modified: Thu, 03 Aug 2023 03:03:46 GMT  
		Size: 741.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9f16769ccd60bfc6c37bac170d94eaea8450f86e7037af4bbdd76ffd32dd9c`  
		Last Modified: Thu, 03 Aug 2023 03:03:45 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610602c4cf5517d76cf7f4d8e9441310dbd2ba991dc2a93f94bb0c791e5ba0b3`  
		Last Modified: Thu, 03 Aug 2023 03:03:45 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18677c045c6414523bb2312b313c88a51526e6a391a04e30d03d247b089d724`  
		Last Modified: Thu, 03 Aug 2023 03:03:45 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0adce102afa0b1f44d32dfba2af0957cf3eee275bade93e91635ab108fe7a9`  
		Last Modified: Thu, 03 Aug 2023 03:03:46 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:enterprise` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:191e40485c3d7a0404733af87322a7b02149d074bf1adc03eb8949e17aa62ebd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **636.8 MB (636755632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a0b7899f3ccdee4d8441e1232f6633f1a2d9b4ae1c6c28580194d087884f836`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:13:43 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 01:13:43 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 01:13:43 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 01:14:01 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 03 Aug 2023 01:14:02 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0
# Thu, 03 Aug 2023 01:14:02 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb
# Thu, 03 Aug 2023 01:14:02 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 03 Aug 2023 01:14:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 01:14:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 01:15:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=b44a4d8e577613ad027dbac9830e6123deb7bda22facefe687d6b6e98c86ac66            ;;          'amd64')            CB_SHA256=2fd31b46a6df5ed9c85d3a6cadfb0214e3f928c14ff0b03e6a24652700128328            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 01:15:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 01:15:13 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 01:15:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 01:15:14 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 01:15:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 01:15:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 03 Aug 2023 01:15:15 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 03 Aug 2023 01:15:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 01:15:15 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 01:15:15 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Thu, 03 Aug 2023 01:15:15 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad91e7dfaee3352f726a7133ee4af8e38e1f989f4a537f0618abd00bb4c784e`  
		Last Modified: Thu, 03 Aug 2023 01:18:32 GMT  
		Size: 6.1 MB (6110566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d117fae1bda3d1ce14ae0cf3990cf2156ac7e81f990b54bc4ae483f50d6a6e`  
		Last Modified: Thu, 03 Aug 2023 01:18:31 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d8d44e8dd52499dbe81834a7c9b340f54094d3b65d3b4c324924c8a48d350`  
		Last Modified: Thu, 03 Aug 2023 01:19:14 GMT  
		Size: 603.4 MB (603440121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742a874d02c82e1540e5b6c7ff63495b2312be683041805df65174a1a9bd9b9b`  
		Last Modified: Thu, 03 Aug 2023 01:18:31 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265ac7f9d2f4e2ad03a33ad57c9287d472fc372ac96ed3c4e908b2f0e2245e36`  
		Last Modified: Thu, 03 Aug 2023 01:18:29 GMT  
		Size: 739.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4430dfb88cb992b7c4d808078a7d23f2ff4883b459d0b099adf44f58e3145cb0`  
		Last Modified: Thu, 03 Aug 2023 01:18:29 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e93e4ab3785185d50863b20c222c5bb80dd625a42cd01491ff351314eb78f2`  
		Last Modified: Thu, 03 Aug 2023 01:18:29 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59147a009b35da6ae2cd75b9fc14052375adb5467ab8c193ba79f63cfae342a6`  
		Last Modified: Thu, 03 Aug 2023 01:18:29 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083a640e5a13d39b2c983bb586c2fcd1283a577da7c1c718d014d05e5a281a10`  
		Last Modified: Thu, 03 Aug 2023 01:18:29 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.6`

```console
$ docker pull couchbase@sha256:b1a23eddd21a1d3bcf03fecc66f9f2595cdade8553911f37c08c59c08e830338
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.6` - linux; amd64

```console
$ docker pull couchbase@sha256:0a16bda78c3e9606ea2cc88f614493abc653e5da5e062c9c4f285712aae85856
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.0 MB (532019586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589bca18245972f4357be12cb94952b66ce0f1aa62e7dc4aa36db6e85af56644`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:54:54 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 02:54:54 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 02:54:54 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:55:09 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 03 Aug 2023 03:02:18 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6
# Thu, 03 Aug 2023 03:02:18 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb
# Thu, 03 Aug 2023 03:02:18 GMT
ARG CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa
# Thu, 03 Aug 2023 03:02:18 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 03 Aug 2023 03:02:18 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Thu, 03 Aug 2023 03:02:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 03:02:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 03:03:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 03:03:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 03:03:17 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 03:03:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 03:03:18 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:03:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 03:03:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.6-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.6 CB_SHA256=db7ec6e2d121ab77ca84a2e02b1617d8e5c92fe83b6fedd15ff618d45c0c89aa CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 03 Aug 2023 03:03:19 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 03 Aug 2023 03:03:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 03:03:19 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 03:03:19 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Thu, 03 Aug 2023 03:03:19 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35618df5c9a71269b91577e6aea59155f8edb63501d542ce129979a4d9e328b`  
		Last Modified: Thu, 03 Aug 2023 03:03:49 GMT  
		Size: 6.3 MB (6285930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b3a69a5ad6f03a3f4a445bb2ee9c4b3eae6877f28386015cdfb95c686ca66a`  
		Last Modified: Thu, 03 Aug 2023 03:09:36 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a3e1cb73494f1b9a9da4eba5b1aacfab98db03861d518050814ff6b765384d`  
		Last Modified: Thu, 03 Aug 2023 03:10:20 GMT  
		Size: 497.1 MB (497148623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479a1455825b1e7f46b1f4e3a4f38be68bafaf261c3e966d0b5ece48f30f6a49`  
		Last Modified: Thu, 03 Aug 2023 03:09:36 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa139d04f2ae93d8a126e07633c875b79ea2b8bf98b5ad4a18eb70788109a11`  
		Last Modified: Thu, 03 Aug 2023 03:09:34 GMT  
		Size: 741.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25bc5d9275e08030f28b782d2368a5e3252a5cc6df8c00b530368815c849ba4`  
		Last Modified: Thu, 03 Aug 2023 03:09:35 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3396770093741a604eba6cf3c036039d18e18decae891394cea9780554b0207`  
		Last Modified: Thu, 03 Aug 2023 03:09:34 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11cf9530ca1bdcc8cd1110f975a3abcb9bd2d7689285c9088c2076679f4268e`  
		Last Modified: Thu, 03 Aug 2023 03:09:34 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69688afb0eadca8780963a6a44f6c69899da47010a3627f58dfad0bfbc72dc41`  
		Last Modified: Thu, 03 Aug 2023 03:09:34 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.0.5`

```console
$ docker pull couchbase@sha256:80147874189584c6c23fe09f86bcd02fdd4c68c152e367c89ce929e4c0b35989
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:021ca5807cb24b470c37b2e24f1927e86ab1118c039ab2b99007df983518debc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **616.7 MB (616700977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7beebceb98d2f7b7f01b7cc186b6f63a4c24c64ca51257575cfb43e63b7d33e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:54:54 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 02:54:54 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 02:54:54 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:55:09 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 03 Aug 2023 02:59:44 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5
# Thu, 03 Aug 2023 02:59:44 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb
# Thu, 03 Aug 2023 02:59:44 GMT
ARG CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea
# Thu, 03 Aug 2023 02:59:44 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 03 Aug 2023 02:59:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 02:59:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 03:00:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 03:00:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 03:00:52 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 03:00:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 03:00:53 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 03:00:53 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 03:00:53 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 03 Aug 2023 03:00:54 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 03 Aug 2023 03:00:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 03:00:54 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 03:00:54 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Thu, 03 Aug 2023 03:00:54 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35618df5c9a71269b91577e6aea59155f8edb63501d542ce129979a4d9e328b`  
		Last Modified: Thu, 03 Aug 2023 03:03:49 GMT  
		Size: 6.3 MB (6285930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f23d74a607dd246cb492e41911e0870aa54ce28bc02c98bee7647b0d719301`  
		Last Modified: Thu, 03 Aug 2023 03:07:39 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c02a2d7ad3410f14faf3e87475bb895cc4c735b9e906cb4ee8eece2c43306a`  
		Last Modified: Thu, 03 Aug 2023 03:08:32 GMT  
		Size: 581.8 MB (581830015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd83a76ab988da2237ecc5fb4cdfe8ac30189561e9cfe1fe52a75d0eef7b42cd`  
		Last Modified: Thu, 03 Aug 2023 03:07:39 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413e65edcbdb6f1db1a64c63017c72cb8a5cb4908bcb27875fa45614f7d7e4cd`  
		Last Modified: Thu, 03 Aug 2023 03:07:37 GMT  
		Size: 739.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63b275fb5763131fb757c3fbb603610ea72dc5124b50d40b17035e42b9874bd`  
		Last Modified: Thu, 03 Aug 2023 03:07:37 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd561df3edd02685f9cb39a9b23b7b14c445fed30a6ba42cc398bc7403709c6`  
		Last Modified: Thu, 03 Aug 2023 03:07:37 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d54f51e85ea641e2ad600dfd0b24a55cea21cd042c7bff56117db7e2cc6ab`  
		Last Modified: Thu, 03 Aug 2023 03:07:37 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455d32fa519253eb3b01b31803fe2b627f33be0339edf1df99834c84d52a3aba`  
		Last Modified: Thu, 03 Aug 2023 03:07:37 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.1.5`

```console
$ docker pull couchbase@sha256:d27a35f7be9298397cd7f270f6b655ff10b647bf283a1b87a09291cc951e9922
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise-7.1.5` - linux; amd64

```console
$ docker pull couchbase@sha256:d79a10ae6216fbc9f695c2168b94b7a8a73a15cbf1988176be68405c90c8d198
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **643.4 MB (643404561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acfb11ee5affaa83a7b8bcf7419bd3312f9f9692e62e38296de777413b526be8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:54:54 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 02:54:54 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 02:54:54 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:55:09 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Fri, 04 Aug 2023 00:24:36 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5
# Fri, 04 Aug 2023 00:24:37 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb
# Fri, 04 Aug 2023 00:24:37 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 04 Aug 2023 00:24:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 04 Aug 2023 00:24:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 04 Aug 2023 00:25:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=57ecac55aca0abf1e6f0a62ebdcd24514cf0d87d09498d794b047d533719321a            ;;          'amd64')            CB_SHA256=b4e3a4f7d10b34471a7ba8a03ac658e79778aaf6b091c9c1631a5c4548e102e0            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 04 Aug 2023 00:26:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 04 Aug 2023 00:26:01 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 04 Aug 2023 00:26:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 04 Aug 2023 00:26:02 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 04 Aug 2023 00:26:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 04 Aug 2023 00:26:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 04 Aug 2023 00:26:03 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 04 Aug 2023 00:26:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 04 Aug 2023 00:26:03 GMT
CMD ["couchbase-server"]
# Fri, 04 Aug 2023 00:26:03 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 04 Aug 2023 00:26:03 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35618df5c9a71269b91577e6aea59155f8edb63501d542ce129979a4d9e328b`  
		Last Modified: Thu, 03 Aug 2023 03:03:49 GMT  
		Size: 6.3 MB (6285930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1257a92c9cfb195b5dd450984903a49323dfdc2dfc6a93b28bf017d96da1f62`  
		Last Modified: Fri, 04 Aug 2023 00:26:45 GMT  
		Size: 1.8 KB (1832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f896d6db571df7b05bc58895c4f7eb33357a50e7fd42c82552a5a1b279418a1`  
		Last Modified: Fri, 04 Aug 2023 00:27:39 GMT  
		Size: 608.5 MB (608533596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc1a46db1570a7eab075a4fb15e83ea5953b875947e533c28aa6cac04ac5dc0`  
		Last Modified: Fri, 04 Aug 2023 00:26:45 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da881006ba56a8bba8cab5eabd4d5f75d5da870b55bb6d543b8f914f742c48b0`  
		Last Modified: Fri, 04 Aug 2023 00:26:43 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8670f2149e78c0e3011851211122aaea50e4429c2847b3c1cc8492aa157743c1`  
		Last Modified: Fri, 04 Aug 2023 00:26:43 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99d460e99a3ec9b231bce484f3c5cb00a0db3a74c3a88df0772a76398353013`  
		Last Modified: Fri, 04 Aug 2023 00:26:43 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a36d7a79c35149244f4ebc6b4305f358151715777ecd04f6da1594334fe7316`  
		Last Modified: Fri, 04 Aug 2023 00:26:46 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d74e13a3f853590260bd93f413041f81b384be15a100bd67f09238350db84c7`  
		Last Modified: Fri, 04 Aug 2023 00:26:43 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:enterprise-7.1.5` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:ea591345fa7ed81a45b3f36a8227db3f6d753df3931ec3436916c2505c259000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.6 MB (617567819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:506076be4a8c2b004cd0406167c2fd1151db359a9dc886dba92784012f94dc68`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:13:43 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 01:13:43 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 01:13:43 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 01:14:01 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Fri, 04 Aug 2023 00:53:42 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5
# Fri, 04 Aug 2023 00:53:42 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb
# Fri, 04 Aug 2023 00:53:42 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 04 Aug 2023 00:53:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 04 Aug 2023 00:53:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 04 Aug 2023 00:54:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=57ecac55aca0abf1e6f0a62ebdcd24514cf0d87d09498d794b047d533719321a            ;;          'amd64')            CB_SHA256=b4e3a4f7d10b34471a7ba8a03ac658e79778aaf6b091c9c1631a5c4548e102e0            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 04 Aug 2023 00:54:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 04 Aug 2023 00:54:47 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 04 Aug 2023 00:54:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 04 Aug 2023 00:54:48 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 04 Aug 2023 00:54:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 04 Aug 2023 00:54:49 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.5-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.5 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 04 Aug 2023 00:54:49 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 04 Aug 2023 00:54:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 04 Aug 2023 00:54:49 GMT
CMD ["couchbase-server"]
# Fri, 04 Aug 2023 00:54:49 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 04 Aug 2023 00:54:49 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad91e7dfaee3352f726a7133ee4af8e38e1f989f4a537f0618abd00bb4c784e`  
		Last Modified: Thu, 03 Aug 2023 01:18:32 GMT  
		Size: 6.1 MB (6110566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f21b205b426f8b3797298acb8e8a75ac504273872cd7921181e3ba9e9b9aae8`  
		Last Modified: Fri, 04 Aug 2023 00:55:08 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e28d875d834a20ae5495b7ce03dd1e973a6ef018ebad30c2ae4c564946a31d7`  
		Last Modified: Fri, 04 Aug 2023 00:55:50 GMT  
		Size: 584.3 MB (584252302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3c5c9949e75bf9cd61a65b90d82b46799541cce82143e9bfad5481e62e5486`  
		Last Modified: Fri, 04 Aug 2023 00:55:07 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ab53f93402b9f9d6d5164cafb4cd163f0aa5a8783e8a1e9472160d95bf1fc6`  
		Last Modified: Fri, 04 Aug 2023 00:55:06 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39ee9d005c164ede9fb4b9ad30b287dea61025cc5a6cfb825543e423d17bb33`  
		Last Modified: Fri, 04 Aug 2023 00:55:06 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49fce06a7532519eb2827348dcd266bb968cf19274cf22ac49682f1a46649cd`  
		Last Modified: Fri, 04 Aug 2023 00:55:06 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2c9c5f9bf13ba8153a3b6af6e17cddd2871cd4fc518972516ca13f899b8081`  
		Last Modified: Fri, 04 Aug 2023 00:55:06 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9cec6241af27697a9d9c1caa0e55ecec8da6eb3324d8500ba5b4bba1a63744`  
		Last Modified: Fri, 04 Aug 2023 00:55:06 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.2.1`

```console
$ docker pull couchbase@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:76114e559a863fde21c7b327ac82c3b5e265599e259ea8731f3c739c42e65464
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:772a2c8fcc3e4a65e410053e5b4f1a4c5349da0ccb78de4d458cf91e49719263
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **663.7 MB (663685101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232147af3c363497c044401c3a221e39f18ad490a26bf4efc84e5e972db019c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:54:54 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 02:54:54 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 02:54:54 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:55:09 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 03 Aug 2023 02:55:10 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0
# Thu, 03 Aug 2023 02:55:10 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb
# Thu, 03 Aug 2023 02:55:10 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 03 Aug 2023 02:55:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 02:55:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 02:56:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=b44a4d8e577613ad027dbac9830e6123deb7bda22facefe687d6b6e98c86ac66            ;;          'amd64')            CB_SHA256=2fd31b46a6df5ed9c85d3a6cadfb0214e3f928c14ff0b03e6a24652700128328            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 02:56:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 02:56:26 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 02:56:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 02:56:26 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 02:56:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 02:56:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 03 Aug 2023 02:56:27 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 03 Aug 2023 02:56:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 02:56:28 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 02:56:28 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Thu, 03 Aug 2023 02:56:28 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35618df5c9a71269b91577e6aea59155f8edb63501d542ce129979a4d9e328b`  
		Last Modified: Thu, 03 Aug 2023 03:03:49 GMT  
		Size: 6.3 MB (6285930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76951ffea2eb9305de925d27044022b82719478ca00eb5b6aa7c90bef872ed3a`  
		Last Modified: Thu, 03 Aug 2023 03:03:47 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91aeb93d2aa72ad20c4cf699740572ef7fd37fa590584cbbb57e54731b7b6cad`  
		Last Modified: Thu, 03 Aug 2023 03:04:45 GMT  
		Size: 628.8 MB (628814146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d05cef67ec666d42e81e534724fed4d45134c72ee363e7a29f01a2ce99df6f`  
		Last Modified: Thu, 03 Aug 2023 03:03:47 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f693b82a631465ff6992c15eb0c719a8520cd5aea5e5b792f56780e5198372`  
		Last Modified: Thu, 03 Aug 2023 03:03:46 GMT  
		Size: 741.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9f16769ccd60bfc6c37bac170d94eaea8450f86e7037af4bbdd76ffd32dd9c`  
		Last Modified: Thu, 03 Aug 2023 03:03:45 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610602c4cf5517d76cf7f4d8e9441310dbd2ba991dc2a93f94bb0c791e5ba0b3`  
		Last Modified: Thu, 03 Aug 2023 03:03:45 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18677c045c6414523bb2312b313c88a51526e6a391a04e30d03d247b089d724`  
		Last Modified: Thu, 03 Aug 2023 03:03:45 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0adce102afa0b1f44d32dfba2af0957cf3eee275bade93e91635ab108fe7a9`  
		Last Modified: Thu, 03 Aug 2023 03:03:46 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:latest` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:191e40485c3d7a0404733af87322a7b02149d074bf1adc03eb8949e17aa62ebd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **636.8 MB (636755632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a0b7899f3ccdee4d8441e1232f6633f1a2d9b4ae1c6c28580194d087884f836`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:13:43 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 03 Aug 2023 01:13:43 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 03 Aug 2023 01:13:43 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 01:14:01 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 03 Aug 2023 01:14:02 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0
# Thu, 03 Aug 2023 01:14:02 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb
# Thu, 03 Aug 2023 01:14:02 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 03 Aug 2023 01:14:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 03 Aug 2023 01:14:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 03 Aug 2023 01:15:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=b44a4d8e577613ad027dbac9830e6123deb7bda22facefe687d6b6e98c86ac66            ;;          'amd64')            CB_SHA256=2fd31b46a6df5ed9c85d3a6cadfb0214e3f928c14ff0b03e6a24652700128328            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 03 Aug 2023 01:15:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 03 Aug 2023 01:15:13 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 03 Aug 2023 01:15:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 03 Aug 2023 01:15:14 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 03 Aug 2023 01:15:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 03 Aug 2023 01:15:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 03 Aug 2023 01:15:15 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 03 Aug 2023 01:15:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 01:15:15 GMT
CMD ["couchbase-server"]
# Thu, 03 Aug 2023 01:15:15 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Thu, 03 Aug 2023 01:15:15 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad91e7dfaee3352f726a7133ee4af8e38e1f989f4a537f0618abd00bb4c784e`  
		Last Modified: Thu, 03 Aug 2023 01:18:32 GMT  
		Size: 6.1 MB (6110566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d117fae1bda3d1ce14ae0cf3990cf2156ac7e81f990b54bc4ae483f50d6a6e`  
		Last Modified: Thu, 03 Aug 2023 01:18:31 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d8d44e8dd52499dbe81834a7c9b340f54094d3b65d3b4c324924c8a48d350`  
		Last Modified: Thu, 03 Aug 2023 01:19:14 GMT  
		Size: 603.4 MB (603440121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742a874d02c82e1540e5b6c7ff63495b2312be683041805df65174a1a9bd9b9b`  
		Last Modified: Thu, 03 Aug 2023 01:18:31 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265ac7f9d2f4e2ad03a33ad57c9287d472fc372ac96ed3c4e908b2f0e2245e36`  
		Last Modified: Thu, 03 Aug 2023 01:18:29 GMT  
		Size: 739.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4430dfb88cb992b7c4d808078a7d23f2ff4883b459d0b099adf44f58e3145cb0`  
		Last Modified: Thu, 03 Aug 2023 01:18:29 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e93e4ab3785185d50863b20c222c5bb80dd625a42cd01491ff351314eb78f2`  
		Last Modified: Thu, 03 Aug 2023 01:18:29 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59147a009b35da6ae2cd75b9fc14052375adb5467ab8c193ba79f63cfae342a6`  
		Last Modified: Thu, 03 Aug 2023 01:18:29 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083a640e5a13d39b2c983bb586c2fcd1283a577da7c1c718d014d05e5a281a10`  
		Last Modified: Thu, 03 Aug 2023 01:18:29 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
