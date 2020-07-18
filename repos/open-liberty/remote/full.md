## `open-liberty:full`

```console
$ docker pull open-liberty@sha256:ac28f4c797f4a6a9acec938f313e61b6a6137a638996ef2b92b075c9f7d614d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full` - linux; amd64

```console
$ docker pull open-liberty@sha256:c2a27d0ea2a831437eb9aa7827ee8981f5c8a8dd7b0543ae0c531f532ee1761b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271833836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6388a94564c394cd1198307ad44aa52575189e91fa2269f5b65430c4a487481a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:21:18 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:21:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 17 Jul 2020 22:53:03 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 17 Jul 2020 22:53:04 GMT
ARG OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 17 Jul 2020 22:53:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 17 Jul 2020 22:53:16 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 17 Jul 2020 22:53:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 17 Jul 2020 22:53:41 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 17 Jul 2020 22:53:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 17 Jul 2020 22:53:41 GMT
USER 1001
# Fri, 17 Jul 2020 22:53:41 GMT
EXPOSE 9080 9443
# Fri, 17 Jul 2020 22:53:42 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 17 Jul 2020 22:53:42 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 17 Jul 2020 22:53:52 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Fri, 17 Jul 2020 22:54:26 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262049cebf1b6f60b6dc78a926be5d3a689ba76a6c5c28edc9b195952b98c31f`  
		Last Modified: Fri, 17 Jul 2020 22:23:14 GMT  
		Size: 13.9 MB (13875144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ae3562f54a1abcec2e390aa39c5d1bdd4d797018f8288100ac516ff45ec7e`  
		Last Modified: Fri, 17 Jul 2020 22:25:12 GMT  
		Size: 48.7 MB (48691295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd1c7cabb21604488842a6b70ae3b2b1f4f3f4ab8f3166c7d886a938b470aa`  
		Last Modified: Fri, 17 Jul 2020 22:56:57 GMT  
		Size: 8.4 KB (8355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0a7e5386637638c3baa64552e90f97f3a78b8758988bede3c9aa9cd9ff23dd`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa2164691c4714f263629a04436be551e7f183e34ae362c7cd328f004d6839e`  
		Last Modified: Fri, 17 Jul 2020 22:57:07 GMT  
		Size: 157.8 MB (157783993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9561ae263f5638923b206f0e2fe29e3b990a44216e271332e01860490479fd5`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b0d9ee4b1303ecddcb8c9642dacd16d0ba6ca2667af936583b610dc1abdbd2`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 9.4 KB (9404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78593c7e93c95a24d1067de28c5918f5b0934f1137c1b6ff284a4984214e12b`  
		Last Modified: Fri, 17 Jul 2020 22:56:58 GMT  
		Size: 8.1 MB (8123074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d87ae3bca31579ea606a2a26fda0d2764eed2c473dbd9463ac06b75fd7bd160`  
		Last Modified: Fri, 17 Jul 2020 22:57:11 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5043a1b4004b7c5e00d1325a216ffb151a0097b1772a5819aeddb8b53eab216`  
		Last Modified: Fri, 17 Jul 2020 22:57:14 GMT  
		Size: 16.6 MB (16607884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:406e1fb5b9ecef8a18441c0e8f89bbec097e74f074000763c81ee68aadb90640
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.4 MB (273386132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:533a1b42c71f538f3b60de5ea84664eacb0ba4a27ab3e5c652f9c60855043cec`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:23:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:24:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:24:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 18 Jul 2020 02:01:05 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Sat, 18 Jul 2020 02:01:11 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Sat, 18 Jul 2020 02:01:18 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Sat, 18 Jul 2020 02:01:22 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Sat, 18 Jul 2020 02:01:26 GMT
ARG OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:01:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Sat, 18 Jul 2020 02:01:33 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Sat, 18 Jul 2020 02:01:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 18 Jul 2020 02:02:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 18 Jul 2020 02:02:36 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:03:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 18 Jul 2020 02:03:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 18 Jul 2020 02:04:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 18 Jul 2020 02:04:11 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 18 Jul 2020 02:04:14 GMT
USER 1001
# Sat, 18 Jul 2020 02:04:19 GMT
EXPOSE 9080 9443
# Sat, 18 Jul 2020 02:04:21 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 18 Jul 2020 02:04:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Sat, 18 Jul 2020 02:04:40 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Sat, 18 Jul 2020 02:05:59 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa43882d8fd530416f9c313375005f26b3e32c8de56ef714a969cea393c840`  
		Last Modified: Fri, 17 Jul 2020 22:29:17 GMT  
		Size: 14.5 MB (14519008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619f87564e3f3e7b4085ba86ac2983c16c46479b5a7e4f631e9f17b63528f7c`  
		Last Modified: Fri, 17 Jul 2020 22:32:27 GMT  
		Size: 49.2 MB (49150050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b16980667b6cf257f5dffb0289980883ce112dc23cb032c08489b48b3df88e`  
		Last Modified: Sat, 18 Jul 2020 02:17:54 GMT  
		Size: 8.4 KB (8382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a72a6ebb235b8952f22c24a95fa8543f80e8c58c15af372b95129e1e820a4`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3153ba5a4e1d3114b68ea85e4be3a97a70f5306da92bc0f21fd6715c8b2863ad`  
		Last Modified: Sat, 18 Jul 2020 02:18:05 GMT  
		Size: 157.8 MB (157785172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56717cde9ea5691083686031ff9d7c0081c78d19166876973b02393a08489ebe`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea378b21197e77bf2f0ef4aebdf4c637d53e68998641b9b4c270315e1fab7cf1`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 9.5 KB (9517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adeb21baf9321364d6aac56520d1c15a64bda2c48ad9d6de03495adf81daad0`  
		Last Modified: Sat, 18 Jul 2020 02:17:52 GMT  
		Size: 6.9 MB (6867452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3d863d3bbe2fba0007496e6d28cb1c228903d11def1649cd0740212c126e4`  
		Last Modified: Sat, 18 Jul 2020 02:18:20 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9473bd9c8be011b5c4fbaff984fdbbcdff651c5e34dbab19e442959b69d8658`  
		Last Modified: Sat, 18 Jul 2020 02:18:23 GMT  
		Size: 14.6 MB (14604611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; s390x

```console
$ docker pull open-liberty@sha256:1b2e122777d5cef35e35f640cdf11d7c7e08ffb961c8728578b3f1fc70769d48
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.2 MB (269174082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:200fcd7bdcf9cf3cd536502362e22fdd4e914a97bd2408b734d2c1b5823f8c53`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 21:07:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 06 Jul 2020 21:07:19 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:09:41 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 06 Jul 2020 21:10:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 06 Jul 2020 21:10:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 06 Jul 2020 21:10:08 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 06 Jul 2020 22:09:29 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Mon, 06 Jul 2020 22:09:29 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Mon, 06 Jul 2020 22:09:30 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Mon, 06 Jul 2020 22:09:30 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Mon, 06 Jul 2020 22:09:30 GMT
ARG OPENJ9_SCC=true
# Mon, 06 Jul 2020 22:09:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Mon, 06 Jul 2020 22:09:30 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Mon, 06 Jul 2020 22:09:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Mon, 06 Jul 2020 22:09:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Mon, 06 Jul 2020 22:09:47 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Mon, 06 Jul 2020 22:09:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 06 Jul 2020 22:09:48 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Mon, 06 Jul 2020 22:10:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Mon, 06 Jul 2020 22:10:02 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Mon, 06 Jul 2020 22:10:02 GMT
USER 1001
# Mon, 06 Jul 2020 22:10:02 GMT
EXPOSE 9080 9443
# Mon, 06 Jul 2020 22:10:03 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Mon, 06 Jul 2020 22:10:03 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Mon, 06 Jul 2020 22:10:12 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Mon, 06 Jul 2020 22:10:30 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4752791f924c0ee1b53766356e35e30e455d055f61cca41c86a87d9bea3f57`  
		Last Modified: Mon, 06 Jul 2020 21:12:59 GMT  
		Size: 13.0 MB (13032773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a900f4e5ca49aca85860e401ba278f074eb46d543d25bb9dd1e5ae31a61b6d`  
		Last Modified: Mon, 06 Jul 2020 21:15:32 GMT  
		Size: 48.3 MB (48289527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05610aaa6cf0d9354cf5b31909df195d2220a484ddac28f1ef5e7132f7feb4d3`  
		Last Modified: Mon, 06 Jul 2020 22:12:49 GMT  
		Size: 8.4 KB (8379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65822a58a7e21cb6ca13813906eded856809d4c01ee51eb8f83a58277dd3090d`  
		Last Modified: Mon, 06 Jul 2020 22:12:47 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d96a8e026b278c8b1fcb4c3847a1375b0e62f3ea66b07b1a8a8abc8e9876ee2`  
		Last Modified: Mon, 06 Jul 2020 22:12:55 GMT  
		Size: 157.7 MB (157725651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ae13f07ec5dd4f9143c305a36d704b17c5796339b1d0bed1c5eac1b4f98dba`  
		Last Modified: Mon, 06 Jul 2020 22:13:03 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23f4e5fbec5f916631c80fd2e3918a1b54ef80fbe6fe8edd054ae038b61c87c`  
		Last Modified: Mon, 06 Jul 2020 22:12:47 GMT  
		Size: 9.5 KB (9499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639003fae4891a84bd4e889a9ab036a64ac85e85d761c43bdecdb8893f0ec9b2`  
		Last Modified: Mon, 06 Jul 2020 22:12:48 GMT  
		Size: 8.1 MB (8147592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9619580e7e007c25b24c8884322b5797917ee81ba2fe1ff240ad5a7883a5387f`  
		Last Modified: Mon, 06 Jul 2020 22:13:07 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acfaa48df30a81eb26d6a25c6ac2aeb35584478d8ff8f2514af00ca99a74dc1`  
		Last Modified: Mon, 06 Jul 2020 22:13:09 GMT  
		Size: 16.6 MB (16552039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
