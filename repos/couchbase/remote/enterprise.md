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
