## `couchbase:community`

```console
$ docker pull couchbase@sha256:13172d60b807fd800a0ee4096154961e3028d34fd5a543a9b8e3b65ed3a4d61b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:3fcddbfc6fab5eae1daddfdcbefb7bfa7bdad89b696d296922ae607da2c4cdd5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357144124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e81e04fed88004119b215eb53f281ac61c863fcfe756f2df769a925fc3795c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:58:57 GMT
LABEL maintainer=docker@couchbase.com
# Fri, 16 Jun 2023 01:58:57 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Fri, 16 Jun 2023 01:58:57 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 16 Jun 2023 01:59:25 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Fri, 16 Jun 2023 01:59:25 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0
# Fri, 16 Jun 2023 02:00:51 GMT
ARG CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb
# Fri, 16 Jun 2023 02:00:51 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 16 Jun 2023 02:00:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 16 Jun 2023 02:00:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 16 Jun 2023 02:01:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=0877ec5c4109992fc2186ecf6153d7f30a24be7f6559133c855ecff77b9b2363            ;;          'amd64')            CB_SHA256=6c07122d9e28c0679c012cba73c28df76a74424cf206fedf42c7e18fa640b6b1            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 16 Jun 2023 02:01:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 16 Jun 2023 02:01:37 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 16 Jun 2023 02:01:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 16 Jun 2023 02:01:37 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 16 Jun 2023 02:01:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 16 Jun 2023 02:01:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 16 Jun 2023 02:01:38 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 16 Jun 2023 02:01:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 02:01:39 GMT
CMD ["couchbase-server"]
# Fri, 16 Jun 2023 02:01:39 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 16 Jun 2023 02:01:39 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6415ade50a8971f892e9c651c561cf94f9aa5d1d59773d9bfcb7c41680c6fe81`  
		Last Modified: Fri, 16 Jun 2023 02:08:02 GMT  
		Size: 6.3 MB (6285956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe8efaf49712b1f6a7b728e1dddd5d3d1c7df4281ead9f234ffc4c6e341aa7`  
		Last Modified: Fri, 16 Jun 2023 02:09:11 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b934484bbb25bcc6bc2d26db24f875a159efdee63472d472a87e662da05ac9ba`  
		Last Modified: Fri, 16 Jun 2023 02:09:47 GMT  
		Size: 322.3 MB (322273284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2d372eea94207b5f4dd316e3c727e386af86fdd58ec6cfe39e78868d439fac`  
		Last Modified: Fri, 16 Jun 2023 02:09:11 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3985dcf9e152f8ac217d515d099661b94a4366d546ba70bf012706e8b2f79f0`  
		Last Modified: Fri, 16 Jun 2023 02:09:09 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4454440ea320671821bdbf539818e5729ec4735cc4f6e5cd958741ef746ecf`  
		Last Modified: Fri, 16 Jun 2023 02:09:09 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c728ce07d9993792434879dad486761884887709813c5cb9f3e4d9edf2f53db2`  
		Last Modified: Fri, 16 Jun 2023 02:09:09 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579d805abb8cca27b227d281c555f11133e79d1912189db4fbf6134fedb03be9`  
		Last Modified: Fri, 16 Jun 2023 02:09:09 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03da2c88e4f2e65dc371191c7a0e7bc89daf6555044468cae7644db2c33855ee`  
		Last Modified: Fri, 16 Jun 2023 02:09:09 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:6353d2eaa2d8bb94764c25f358aca9407ba16adbefc6d8027d956a35317af988
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.6 MB (335640747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b400a47c5043c360f1b5185e43b42e0cbd7915430b37eeb3f398586e48b811fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:37:07 GMT
LABEL maintainer=docker@couchbase.com
# Fri, 16 Jun 2023 02:37:07 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Fri, 16 Jun 2023 02:37:07 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 16 Jun 2023 02:37:32 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Fri, 16 Jun 2023 02:37:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0
# Fri, 16 Jun 2023 02:38:45 GMT
ARG CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb
# Fri, 16 Jun 2023 02:38:45 GMT
ARG CB_SKIP_CHECKSUM=false
# Fri, 16 Jun 2023 02:38:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 16 Jun 2023 02:38:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 16 Jun 2023 02:39:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=0877ec5c4109992fc2186ecf6153d7f30a24be7f6559133c855ecff77b9b2363            ;;          'amd64')            CB_SHA256=6c07122d9e28c0679c012cba73c28df76a74424cf206fedf42c7e18fa640b6b1            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 16 Jun 2023 02:39:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 16 Jun 2023 02:39:24 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 16 Jun 2023 02:39:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 16 Jun 2023 02:39:24 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 16 Jun 2023 02:39:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 16 Jun 2023 02:39:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.2.0-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.2.0 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 16 Jun 2023 02:39:25 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 16 Jun 2023 02:39:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 02:39:26 GMT
CMD ["couchbase-server"]
# Fri, 16 Jun 2023 02:39:26 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Fri, 16 Jun 2023 02:39:26 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8a2d2e9bc2c1acc384514d4e79ba7b79369a7c6c1d8fb1dec63484dc162b6f`  
		Last Modified: Fri, 16 Jun 2023 02:41:54 GMT  
		Size: 6.1 MB (6110610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6d0557f6f7baa258e3aa88e04d94c8bf9dfb6a273098d9d9babd308d2209c9`  
		Last Modified: Fri, 16 Jun 2023 02:42:47 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb3c8edc4da8fad3ddb886d581854588872de6077964b440c26c1f3b3a60245`  
		Last Modified: Fri, 16 Jun 2023 02:43:16 GMT  
		Size: 302.3 MB (302325339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ed9be0be41aaea6d478d82eba0bcecbdc298f562d8e9b258cdfaf896f3b32d`  
		Last Modified: Fri, 16 Jun 2023 02:42:47 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b7973ac11045238409a3a9b795256eb96bbbf356122a7715ec081e68b49b1f`  
		Last Modified: Fri, 16 Jun 2023 02:42:45 GMT  
		Size: 741.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406d289984a75de8fad0a162e638d9db8171af2726608aceeda830b8dff44ca3`  
		Last Modified: Fri, 16 Jun 2023 02:42:45 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d7c920075fc03a32cda21610c3651596ac9e581ac0e62aeb415143d9011479`  
		Last Modified: Fri, 16 Jun 2023 02:42:45 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381f2416589dd33c7d24269bc45ea2dae4cc01499549bc80f6adc6a3c182dd3a`  
		Last Modified: Fri, 16 Jun 2023 02:42:45 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c9748f9e440e371c62fbee6fe4227feb8b081509a67fc01582bf9b739b0ef6`  
		Last Modified: Fri, 16 Jun 2023 02:42:45 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
