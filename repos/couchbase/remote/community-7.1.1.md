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
