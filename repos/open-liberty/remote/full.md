## `open-liberty:full`

```console
$ docker pull open-liberty@sha256:4897756ce39b921c52ac18cc7f88abd0778b64637f6a180d860a53a3fca2eb85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full` - linux; amd64

```console
$ docker pull open-liberty@sha256:d65f91d532f7e9213a035ca9c5a6084044d50034c8b95710c0a816131cb18ac0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269635041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d806902bd816ca31ab3171c8dda4d9cb0e8305b16e92f065902c9b1f8f66e408`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 19:27:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Apr 2020 19:28:13 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 19:29:59 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Fri, 24 Apr 2020 19:30:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Apr 2020 19:30:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Apr 2020 19:30:18 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 13 May 2020 01:21:36 GMT
ARG LIBERTY_VERSION=20.0.0.5
# Wed, 13 May 2020 01:21:36 GMT
ARG LIBERTY_SHA=bd1909170f3ef9723e4ab9a7a3b6273b846b1974
# Wed, 13 May 2020 01:21:36 GMT
ARG LIBERTY_BUILD_LABEL=cl200520200429-1655
# Wed, 13 May 2020 01:21:36 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.5/openliberty-runtime-20.0.0.5.zip
# Wed, 13 May 2020 01:21:37 GMT
ARG OPENJ9_SCC=true
# Wed, 13 May 2020 01:21:37 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200520200429-1655 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.5
# Sat, 16 May 2020 08:09:17 GMT
COPY dir:3972e7c0b5a02ecce167022cd7d99f08a97f0c64258f1006db044bc7a25fef99 in /opt/ol/helpers 
# Sat, 16 May 2020 08:09:17 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 16 May 2020 08:09:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200520200429-1655 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.5/openliberty-runtime-20.0.0.5.zip LIBERTY_SHA=bd1909170f3ef9723e4ab9a7a3b6273b846b1974 LIBERTY_VERSION=20.0.0.5 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 16 May 2020 08:09:34 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 16 May 2020 08:09:35 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200520200429-1655 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.5/openliberty-runtime-20.0.0.5.zip LIBERTY_SHA=bd1909170f3ef9723e4ab9a7a3b6273b846b1974 LIBERTY_VERSION=20.0.0.5
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 16 May 2020 08:09:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200520200429-1655 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.5/openliberty-runtime-20.0.0.5.zip LIBERTY_SHA=bd1909170f3ef9723e4ab9a7a3b6273b846b1974 LIBERTY_VERSION=20.0.0.5
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 16 May 2020 08:09:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200520200429-1655 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.5/openliberty-runtime-20.0.0.5.zip LIBERTY_SHA=bd1909170f3ef9723e4ab9a7a3b6273b846b1974 LIBERTY_VERSION=20.0.0.5
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 16 May 2020 08:09:57 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 16 May 2020 08:09:57 GMT
USER 1001
# Sat, 16 May 2020 08:09:58 GMT
EXPOSE 9080 9443
# Sat, 16 May 2020 08:09:58 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 16 May 2020 08:09:58 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Sat, 16 May 2020 08:10:05 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Sat, 16 May 2020 08:10:37 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3058952867bac0b1deeecce925b304f4e354c7b8781d75fbfc6d36373ead53af`  
		Last Modified: Fri, 24 Apr 2020 19:32:11 GMT  
		Size: 13.3 MB (13324407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ca17f7600d2906e0183fa0288c8a744578c210727ae22c06d4b22c180b0e6`  
		Last Modified: Fri, 24 Apr 2020 19:34:47 GMT  
		Size: 48.5 MB (48502686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c0a578b17cb33ebad8b21035e2b90067e53734cc25380d9b5c8abeafbdbb2d`  
		Last Modified: Sat, 16 May 2020 08:11:51 GMT  
		Size: 8.0 KB (8017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507e18760fdea427d8c17ef5a297ddf07ac65b75b58255010db553e118cedfb5`  
		Last Modified: Sat, 16 May 2020 08:11:51 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df8c45cffc577c31b998170905676d7d9016f42e5659c92a43a0f7f60c54039`  
		Last Modified: Sat, 16 May 2020 08:12:01 GMT  
		Size: 156.0 MB (156009368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da47514e59a75615ec704feeefee2992ab7c21b573748f330c504a113385793b`  
		Last Modified: Sat, 16 May 2020 08:11:50 GMT  
		Size: 909.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debfef74bb09288f8f99894d4525f7c7d838c2c4f1ef42482e9746dc12b99121`  
		Last Modified: Sat, 16 May 2020 08:11:50 GMT  
		Size: 9.1 KB (9068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8577cd6811dfde68233c5bdf8db62d3077970397f3db0b61b910f7daa091fb61`  
		Last Modified: Sat, 16 May 2020 08:11:52 GMT  
		Size: 8.2 MB (8178044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8953a237b5736612112c474d78a543a1ed394c75b96eb7287895b2b5ba66432`  
		Last Modified: Sat, 16 May 2020 08:12:06 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09316634f9387f5c2316524d21dcd30d513b9e387edaf9e30966f1c295f02c66`  
		Last Modified: Sat, 16 May 2020 08:12:09 GMT  
		Size: 16.9 MB (16875170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:5a3be01b3e029d05d6bf0f69a80b1e9dd59ba5bc593684807c0def66d38ab1d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.9 MB (270871770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f04d218579269e1b3caf0bdac67fd1f0c77a65ca8d5c9fbc672beb863b73b745`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 23 Apr 2020 20:42:30 GMT
ADD file:726a32203fbcaae787c10740754e38dcb186778893e6d078db3cba0f49ee6b3c in / 
# Thu, 23 Apr 2020 20:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 20:42:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 20:42:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 20:42:50 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:22:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Apr 2020 11:23:45 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:28:55 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Fri, 24 Apr 2020 11:29:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Apr 2020 11:29:59 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Apr 2020 11:30:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 13 May 2020 01:21:42 GMT
ARG LIBERTY_VERSION=20.0.0.5
# Wed, 13 May 2020 01:21:45 GMT
ARG LIBERTY_SHA=bd1909170f3ef9723e4ab9a7a3b6273b846b1974
# Wed, 13 May 2020 01:21:47 GMT
ARG LIBERTY_BUILD_LABEL=cl200520200429-1655
# Wed, 13 May 2020 01:21:52 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.5/openliberty-runtime-20.0.0.5.zip
# Wed, 13 May 2020 01:21:54 GMT
ARG OPENJ9_SCC=true
# Wed, 13 May 2020 01:21:57 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200520200429-1655 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.5
# Sat, 16 May 2020 18:49:34 GMT
COPY dir:3972e7c0b5a02ecce167022cd7d99f08a97f0c64258f1006db044bc7a25fef99 in /opt/ol/helpers 
# Sat, 16 May 2020 18:49:39 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Mon, 18 May 2020 07:25:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200520200429-1655 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.5/openliberty-runtime-20.0.0.5.zip LIBERTY_SHA=bd1909170f3ef9723e4ab9a7a3b6273b846b1974 LIBERTY_VERSION=20.0.0.5 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Mon, 18 May 2020 07:25:11 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Mon, 18 May 2020 07:25:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200520200429-1655 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.5/openliberty-runtime-20.0.0.5.zip LIBERTY_SHA=bd1909170f3ef9723e4ab9a7a3b6273b846b1974 LIBERTY_VERSION=20.0.0.5
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 18 May 2020 07:25:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200520200429-1655 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.5/openliberty-runtime-20.0.0.5.zip LIBERTY_SHA=bd1909170f3ef9723e4ab9a7a3b6273b846b1974 LIBERTY_VERSION=20.0.0.5
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Mon, 18 May 2020 07:25:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200520200429-1655 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.5/openliberty-runtime-20.0.0.5.zip LIBERTY_SHA=bd1909170f3ef9723e4ab9a7a3b6273b846b1974 LIBERTY_VERSION=20.0.0.5
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Mon, 18 May 2020 07:26:04 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Mon, 18 May 2020 07:26:09 GMT
USER 1001
# Mon, 18 May 2020 07:26:12 GMT
EXPOSE 9080 9443
# Mon, 18 May 2020 07:26:17 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Mon, 18 May 2020 07:26:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Mon, 18 May 2020 07:26:50 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Mon, 18 May 2020 07:27:40 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:beed3bd0a281cacead564771f079ed9ee8b272a2ed0e28f533e188f3d21fee6e`  
		Last Modified: Mon, 06 Apr 2020 15:40:20 GMT  
		Size: 30.4 MB (30400298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14d2411b83450b8afe92058b998540c56ec42f1ddd7581e8e9fe629c442f89`  
		Last Modified: Thu, 23 Apr 2020 20:48:44 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82678240be3a5c783512ff7336f2b10837ae126958bc6bd1b476a8d039c08771`  
		Last Modified: Thu, 23 Apr 2020 20:48:44 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7307ad4f24078fd763b41ec7c1772f2fd5238fed1bae36c5d42d28ec9adbffb9`  
		Last Modified: Thu, 23 Apr 2020 20:48:44 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841fc1003510ef9b0e7994850d1dd2608238f020eb8892ebb14f71b9b02c1170`  
		Last Modified: Fri, 24 Apr 2020 11:36:20 GMT  
		Size: 14.0 MB (13970642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d45e0c4fcddd15c749661cc0058c2dd7920e760df9db2dffdc965e2ef971479`  
		Last Modified: Fri, 24 Apr 2020 11:42:31 GMT  
		Size: 49.0 MB (48992426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2920137e4f91125ca106fd05bf85e6ba54d77c6a2feae6cb3625c3adcc83bed`  
		Last Modified: Mon, 18 May 2020 07:34:10 GMT  
		Size: 8.0 KB (8049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc046d457827dca5c85ef59a94d88eba19073abb2f572a44b7dc4c2d0b315789`  
		Last Modified: Mon, 18 May 2020 07:34:07 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce90d0ef4a16bde383b47ddffa03e61b1a81eb21cbb9ae86a676a98be4d752e`  
		Last Modified: Mon, 18 May 2020 07:34:43 GMT  
		Size: 156.0 MB (156010121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5811a8c960fee545a13adb0d30d32ea7e5e8031bbfb327a60202d89d587bc15f`  
		Last Modified: Mon, 18 May 2020 07:34:06 GMT  
		Size: 971.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7d03dd8f1a8dfdf10cf5af3c6829e6b3b0f44936ab70c597817b62f11fcf62`  
		Last Modified: Mon, 18 May 2020 07:34:07 GMT  
		Size: 9.2 KB (9189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10ffa80a75dd4454379a0fdb59648f0e9fa918c05da879fd3c12ba864ed93dc`  
		Last Modified: Mon, 18 May 2020 07:34:08 GMT  
		Size: 6.9 MB (6876989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cef7047252db7c222c8c042ff6eb474aa0c53f88d748c6cb73458f6c4060a7`  
		Last Modified: Mon, 18 May 2020 07:34:55 GMT  
		Size: 971.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74a8284a8915854e8fb80e862e3a3ea1796ce50971e836ff9df4079a504c65e`  
		Last Modified: Mon, 18 May 2020 07:34:59 GMT  
		Size: 14.6 MB (14565609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; s390x

```console
$ docker pull open-liberty@sha256:7d522fc6abb71f133940bac8c18db2390da539d7dbe5954f172cb593d3b5200f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.2 MB (269219265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1988e014dde157e44f6b74ca4b15ced42f20137175321c046e7445e858cc63`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 23 Apr 2020 17:52:20 GMT
ADD file:ea66ef2a01c547f771866bfa221969f8a30489c28d2a81be8dde7f40e73da33b in / 
# Thu, 23 Apr 2020 17:52:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 17:52:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:52:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:52:31 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:36:55 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Apr 2020 07:37:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:39:14 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Fri, 24 Apr 2020 07:39:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Apr 2020 07:39:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Apr 2020 07:39:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 05 Jun 2020 22:41:44 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Fri, 05 Jun 2020 22:41:44 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Fri, 05 Jun 2020 22:41:45 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Fri, 05 Jun 2020 22:41:45 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Fri, 05 Jun 2020 22:41:45 GMT
ARG OPENJ9_SCC=true
# Fri, 05 Jun 2020 22:41:45 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Fri, 05 Jun 2020 22:41:45 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 05 Jun 2020 22:41:46 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 05 Jun 2020 22:41:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 05 Jun 2020 22:42:00 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 05 Jun 2020 22:42:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 05 Jun 2020 22:42:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 05 Jun 2020 22:42:15 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 05 Jun 2020 22:42:15 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 05 Jun 2020 22:42:15 GMT
USER 1001
# Fri, 05 Jun 2020 22:42:16 GMT
EXPOSE 9080 9443
# Fri, 05 Jun 2020 22:42:16 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 05 Jun 2020 22:42:16 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 05 Jun 2020 22:42:21 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Fri, 05 Jun 2020 22:42:39 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:13b4c2e4bb97a2a80bb0e557eeba41e4adea0f5e18352e359bca3f847193899c`  
		Last Modified: Mon, 06 Apr 2020 15:41:16 GMT  
		Size: 25.4 MB (25365338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471a80e39fb485b86610de915eaaad3d867cc97e460b6da3bb656e03520e8a63`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 36.2 KB (36171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb0c128ddabc6a980ec71426ade04fc9bba2e1afcdc243e2d09c316b635f814`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678052ac148ee123df2f0773eb3a0f5f90490ada8b9a5705363b18a2f45fbe88`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cda817e3f7c865b0840c4d8029ccd310418aaf7af7a0aeda3eaa4cb945fca4b`  
		Last Modified: Fri, 24 Apr 2020 07:41:58 GMT  
		Size: 13.0 MB (13043886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fffe5699c9d3c03456957c9977d42c3622c4b7180850d773a72dbc3a7e9c06`  
		Last Modified: Fri, 24 Apr 2020 07:44:28 GMT  
		Size: 48.3 MB (48289486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0079b58864bf52ba165ca3da9d3b1fc7e9d04fd0de9c63d674e105370ac49262`  
		Last Modified: Fri, 05 Jun 2020 22:43:09 GMT  
		Size: 8.4 KB (8378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25ba5511f259e116bd484b4d4dfaab9fbe3a91388a136a0f59263833cd48dc9`  
		Last Modified: Fri, 05 Jun 2020 22:43:08 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ec29db81ee7f97e44ff548ac75bd7a86b4be307ef6c9bc20a92a3c25c767ba`  
		Last Modified: Fri, 05 Jun 2020 22:43:20 GMT  
		Size: 158.0 MB (158012423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed279bdf64f9f5e8360eb8dbeccc3ef080a7f9c642378ef0cf6d4f28d15b2c5`  
		Last Modified: Fri, 05 Jun 2020 22:43:08 GMT  
		Size: 969.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721cbb96002caafd341f797bf9f936a34de796b593f31491a45e672588441378`  
		Last Modified: Fri, 05 Jun 2020 22:43:08 GMT  
		Size: 9.5 KB (9494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328473982beaa27e708f5472c5cbfb7d8ab1071d4bf72528265a3a44a6b2b72a`  
		Last Modified: Fri, 05 Jun 2020 22:43:09 GMT  
		Size: 8.0 MB (8001119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5633b33eb0354b92cc4b220f07e18194861425a2d794fe3d2ed9af843957cab1`  
		Last Modified: Fri, 05 Jun 2020 22:43:26 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b07eee2d852b39de9a109edbbfb88cf917068b70520c95030021aa8b749ff7`  
		Last Modified: Fri, 05 Jun 2020 22:43:28 GMT  
		Size: 16.4 MB (16449735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
