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
