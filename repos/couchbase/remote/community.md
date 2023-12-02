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
