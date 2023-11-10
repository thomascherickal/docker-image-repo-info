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
