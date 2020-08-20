<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `open-liberty`

-	[`open-liberty:20.0.0.3-full-java8-openj9`](#open-liberty20003-full-java8-openj9)
-	[`open-liberty:20.0.0.3-kernel-java8-openj9`](#open-liberty20003-kernel-java8-openj9)
-	[`open-liberty:20.0.0.6-full-java8-openj9`](#open-liberty20006-full-java8-openj9)
-	[`open-liberty:20.0.0.6-kernel-java8-openj9`](#open-liberty20006-kernel-java8-openj9)
-	[`open-liberty:20.0.0.8-full-java8-openj9`](#open-liberty20008-full-java8-openj9)
-	[`open-liberty:20.0.0.8-kernel-java8-openj9`](#open-liberty20008-kernel-java8-openj9)
-	[`open-liberty:full`](#open-libertyfull)
-	[`open-liberty:full-java8-openj9`](#open-libertyfull-java8-openj9)
-	[`open-liberty:kernel`](#open-libertykernel)
-	[`open-liberty:kernel-java8-openj9`](#open-libertykernel-java8-openj9)
-	[`open-liberty:latest`](#open-libertylatest)

## `open-liberty:20.0.0.3-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:ef98f179aab11e3cc88ddee7daa23bcf1336b841d36717694d05fde5e311555b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.3-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:a3355d12ba6551ebdf95fa221f5584e476feefede90da446bcc312150e59b46e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.7 MB (252705342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd6604e1ed62451bdee0afa39b279be1958ed22f6e46f646eca567d6eb2efe0a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:00:38 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 02:19:30 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Thu, 20 Aug 2020 02:19:30 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Thu, 20 Aug 2020 02:19:30 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Thu, 20 Aug 2020 02:19:30 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Thu, 20 Aug 2020 02:19:30 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:19:31 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.3
# Thu, 20 Aug 2020 02:19:31 GMT
COPY dir:db13e0b286891a0bd7aa45ab6285056101f78bde154aff1711d0e2933840a07f in /opt/ol/helpers 
# Thu, 20 Aug 2020 02:19:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 02:19:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 02:19:43 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:19:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 02:19:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 02:20:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 02:20:04 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 02:20:05 GMT
USER 1001
# Thu, 20 Aug 2020 02:20:05 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 02:20:05 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 02:20:05 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 02:20:10 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a8737f865890826d26efd4c158416bd1188e715c783fd41548e040ef975dbe`  
		Last Modified: Wed, 19 Aug 2020 22:05:50 GMT  
		Size: 48.7 MB (48691306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2a86eeb989bac47aa0d7dec283c618831f9ba1a3d5aee98669dcb0a103f18c`  
		Last Modified: Thu, 20 Aug 2020 02:21:08 GMT  
		Size: 6.5 KB (6521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439cad3c72555052a905974f4075978cbcd5347c01569baaa0cb1b11c44bb5a1`  
		Last Modified: Thu, 20 Aug 2020 02:21:07 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60489c3824772791bb9e13e3565f38c4d0bf7406c18a7649b57adc82d9022b63`  
		Last Modified: Thu, 20 Aug 2020 02:21:17 GMT  
		Size: 155.1 MB (155084996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44406c4aa48881fc147360ecb7c916b67845d0ed041444147d47967f094d59`  
		Last Modified: Thu, 20 Aug 2020 02:21:07 GMT  
		Size: 937.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0da44c3ce5d2ab34896da4d274b3bcb09c870277fcfc1080d9183a4931505d`  
		Last Modified: Thu, 20 Aug 2020 02:21:07 GMT  
		Size: 7.6 KB (7554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74288dbd9f229c2d0fb5fe80e3d6545f41c0a9ac75119864288320ceb21cd1b3`  
		Last Modified: Thu, 20 Aug 2020 02:21:09 GMT  
		Size: 8.3 MB (8301163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e1e021523709ce49334d5078358e8c7dadec59a93fc81c6c9090c3f09cb544`  
		Last Modified: Thu, 20 Aug 2020 02:21:20 GMT  
		Size: 961.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.3-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:ccfe51afb84b548c5f0551bb5423a8068a62dcc5140baca311339265c8335794
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.1 MB (256120238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:281b55d9f9df0a98f83ea80ff1793a4ac6eeae040fd6f1969fbe8951c4a42ab0`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:33 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:33:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:33:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:33:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 03:22:58 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Thu, 20 Aug 2020 03:23:01 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Thu, 20 Aug 2020 03:23:03 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Thu, 20 Aug 2020 03:23:06 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Thu, 20 Aug 2020 03:23:11 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:23:14 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.3
# Thu, 20 Aug 2020 03:23:17 GMT
COPY dir:db13e0b286891a0bd7aa45ab6285056101f78bde154aff1711d0e2933840a07f in /opt/ol/helpers 
# Thu, 20 Aug 2020 03:23:18 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 03:23:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 03:23:57 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:24:14 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 03:24:31 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 03:25:01 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 03:25:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 03:25:11 GMT
USER 1001
# Thu, 20 Aug 2020 03:25:16 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 03:25:20 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 03:25:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 03:25:43 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59a1586230e65d6fbe8aebe774b944895c099ea81decb8818ba03aa8180880`  
		Last Modified: Wed, 19 Aug 2020 22:46:13 GMT  
		Size: 49.2 MB (49150099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86356038d993f5c83f12ce34f55daf1ed86277487e0d2a5ae711d7b98710df24`  
		Last Modified: Thu, 20 Aug 2020 03:27:36 GMT  
		Size: 6.5 KB (6547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5340caf8e711f319d5cbac17d8a83623c12949d99b6d3548a159e8ee87a1e6`  
		Last Modified: Thu, 20 Aug 2020 03:27:29 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895b9f1f14f2bb12a1d90080c08e480e31646acbb8f4b00cf1b16330c0a6567c`  
		Last Modified: Thu, 20 Aug 2020 03:28:02 GMT  
		Size: 155.1 MB (155085732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6184205456fb846a8cbccedcc546916f1a19c0ec5c2b37b8f44086a6bf4dd40`  
		Last Modified: Thu, 20 Aug 2020 03:27:29 GMT  
		Size: 1.0 KB (1005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb0aa68d387a3b41335ad627d22c13f077e733d8b3da7642930a35fa6876104`  
		Last Modified: Thu, 20 Aug 2020 03:27:29 GMT  
		Size: 7.7 KB (7662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5036a5b0cd2c4e0ee79b89d5b50adaf6e5833a17321689e6e1927d87c5e91794`  
		Last Modified: Thu, 20 Aug 2020 03:27:31 GMT  
		Size: 6.9 MB (6904033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065f8e30ecc042c28a5e9386bf7395de41a10ba9aaa700832dfa75dab4e59c8e`  
		Last Modified: Thu, 20 Aug 2020 03:28:11 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.3-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:b5a3853bb074874f28e96e0fe70d0e98a8b02b5ceb4567d06f964203bf3adad6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250624507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b17158dbddea36e53eccc0564eb73853845ab697bfef97ff851edcccb7903812`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:22 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 21:59:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:48:45 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Wed, 19 Aug 2020 22:48:45 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Wed, 19 Aug 2020 22:48:45 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Wed, 19 Aug 2020 22:48:45 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Wed, 19 Aug 2020 22:48:46 GMT
ARG OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:48:46 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.3
# Wed, 19 Aug 2020 22:48:46 GMT
COPY dir:db13e0b286891a0bd7aa45ab6285056101f78bde154aff1711d0e2933840a07f in /opt/ol/helpers 
# Wed, 19 Aug 2020 22:48:46 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 19 Aug 2020 22:48:59 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 19 Aug 2020 22:49:03 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:49:05 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 19 Aug 2020 22:49:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 19 Aug 2020 22:49:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 19 Aug 2020 22:49:19 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 19 Aug 2020 22:49:19 GMT
USER 1001
# Wed, 19 Aug 2020 22:49:19 GMT
EXPOSE 9080 9443
# Wed, 19 Aug 2020 22:49:19 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 19 Aug 2020 22:49:20 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Wed, 19 Aug 2020 22:49:27 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172b17642c4976ab19fd089c118bc5daf377f3a385fee3563d8af19598f2050`  
		Last Modified: Wed, 19 Aug 2020 22:05:35 GMT  
		Size: 48.4 MB (48386872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dfa59a43319950ed2738e122529b6b034f798a23077257b0cd1910c40ad574`  
		Last Modified: Wed, 19 Aug 2020 22:50:24 GMT  
		Size: 6.5 KB (6546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8e400b4e985535532b056a643b9ad936a4a2086931734bb02d805f47c0c30c`  
		Last Modified: Wed, 19 Aug 2020 22:50:22 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93bf828038129ec93ba11d0e72783ee2bd2cb09a01f68f92b77abf3abf5fe57`  
		Last Modified: Wed, 19 Aug 2020 22:50:30 GMT  
		Size: 155.1 MB (155084736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fe00d8b21f6d682fb115b5212b386cea20648d1425fd89d94b579a8589a7a0`  
		Last Modified: Wed, 19 Aug 2020 22:50:22 GMT  
		Size: 996.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06ed7665c9f16ef89267c846bcd994f7c0ae50c035437755b0796cc863ab214`  
		Last Modified: Wed, 19 Aug 2020 22:50:22 GMT  
		Size: 7.6 KB (7636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14ac1b48233f0cf20171e3550091564791a1a6ee50181f5a3f317a70745303b`  
		Last Modified: Wed, 19 Aug 2020 22:50:23 GMT  
		Size: 8.1 MB (8132510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89e0ce4ecdad35f1e4311b1a8824b86ed019b35af05c9dc5baa694d3311fa71`  
		Last Modified: Wed, 19 Aug 2020 22:50:35 GMT  
		Size: 965.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.3-kernel-java8-openj9`

```console
$ docker pull open-liberty@sha256:ef18a288bdce9062615da3a447e0d08c2c86fa201701024dedd72459fd8442f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.3-kernel-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:04b061a78e18294f5da1b4f0668c54fc3939fb1c64c263e5f3aaf99c29121eab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.7 MB (252704381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c75ed7a8177efff535de9d24e7ea0b0377fd670db2645103f3c34ea6f45d5d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:00:38 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 02:19:30 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Thu, 20 Aug 2020 02:19:30 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Thu, 20 Aug 2020 02:19:30 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Thu, 20 Aug 2020 02:19:30 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Thu, 20 Aug 2020 02:19:30 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:19:31 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.3
# Thu, 20 Aug 2020 02:19:31 GMT
COPY dir:db13e0b286891a0bd7aa45ab6285056101f78bde154aff1711d0e2933840a07f in /opt/ol/helpers 
# Thu, 20 Aug 2020 02:19:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 02:19:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 02:19:43 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:19:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 02:19:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 02:20:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 02:20:04 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 02:20:05 GMT
USER 1001
# Thu, 20 Aug 2020 02:20:05 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 02:20:05 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 02:20:05 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a8737f865890826d26efd4c158416bd1188e715c783fd41548e040ef975dbe`  
		Last Modified: Wed, 19 Aug 2020 22:05:50 GMT  
		Size: 48.7 MB (48691306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2a86eeb989bac47aa0d7dec283c618831f9ba1a3d5aee98669dcb0a103f18c`  
		Last Modified: Thu, 20 Aug 2020 02:21:08 GMT  
		Size: 6.5 KB (6521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439cad3c72555052a905974f4075978cbcd5347c01569baaa0cb1b11c44bb5a1`  
		Last Modified: Thu, 20 Aug 2020 02:21:07 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60489c3824772791bb9e13e3565f38c4d0bf7406c18a7649b57adc82d9022b63`  
		Last Modified: Thu, 20 Aug 2020 02:21:17 GMT  
		Size: 155.1 MB (155084996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44406c4aa48881fc147360ecb7c916b67845d0ed041444147d47967f094d59`  
		Last Modified: Thu, 20 Aug 2020 02:21:07 GMT  
		Size: 937.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0da44c3ce5d2ab34896da4d274b3bcb09c870277fcfc1080d9183a4931505d`  
		Last Modified: Thu, 20 Aug 2020 02:21:07 GMT  
		Size: 7.6 KB (7554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74288dbd9f229c2d0fb5fe80e3d6545f41c0a9ac75119864288320ceb21cd1b3`  
		Last Modified: Thu, 20 Aug 2020 02:21:09 GMT  
		Size: 8.3 MB (8301163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.3-kernel-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:382e761b4ea93115fb36421ee0f67eb335f0a2cec3053d28bd90b1b38d608489
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.1 MB (256119272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c9e4cebdf1afdfa6b01b99cb85aa8d99ab3a16c8e0666f6b30d7d286a7c937e`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:33 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:33:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:33:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:33:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 03:22:58 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Thu, 20 Aug 2020 03:23:01 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Thu, 20 Aug 2020 03:23:03 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Thu, 20 Aug 2020 03:23:06 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Thu, 20 Aug 2020 03:23:11 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:23:14 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.3
# Thu, 20 Aug 2020 03:23:17 GMT
COPY dir:db13e0b286891a0bd7aa45ab6285056101f78bde154aff1711d0e2933840a07f in /opt/ol/helpers 
# Thu, 20 Aug 2020 03:23:18 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 03:23:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 03:23:57 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:24:14 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 03:24:31 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 03:25:01 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 03:25:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 03:25:11 GMT
USER 1001
# Thu, 20 Aug 2020 03:25:16 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 03:25:20 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 03:25:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59a1586230e65d6fbe8aebe774b944895c099ea81decb8818ba03aa8180880`  
		Last Modified: Wed, 19 Aug 2020 22:46:13 GMT  
		Size: 49.2 MB (49150099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86356038d993f5c83f12ce34f55daf1ed86277487e0d2a5ae711d7b98710df24`  
		Last Modified: Thu, 20 Aug 2020 03:27:36 GMT  
		Size: 6.5 KB (6547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5340caf8e711f319d5cbac17d8a83623c12949d99b6d3548a159e8ee87a1e6`  
		Last Modified: Thu, 20 Aug 2020 03:27:29 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895b9f1f14f2bb12a1d90080c08e480e31646acbb8f4b00cf1b16330c0a6567c`  
		Last Modified: Thu, 20 Aug 2020 03:28:02 GMT  
		Size: 155.1 MB (155085732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6184205456fb846a8cbccedcc546916f1a19c0ec5c2b37b8f44086a6bf4dd40`  
		Last Modified: Thu, 20 Aug 2020 03:27:29 GMT  
		Size: 1.0 KB (1005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb0aa68d387a3b41335ad627d22c13f077e733d8b3da7642930a35fa6876104`  
		Last Modified: Thu, 20 Aug 2020 03:27:29 GMT  
		Size: 7.7 KB (7662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5036a5b0cd2c4e0ee79b89d5b50adaf6e5833a17321689e6e1927d87c5e91794`  
		Last Modified: Thu, 20 Aug 2020 03:27:31 GMT  
		Size: 6.9 MB (6904033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.3-kernel-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:8de6153618fefa466bf074146ef3f3ef14915e8115aa28bf9a51a0d1ae301cea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250623542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cc146ea27ef8690bbcf75c21ddcf5c076745adde53ac51788baeb3ac97f27cd`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:22 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 21:59:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:48:45 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Wed, 19 Aug 2020 22:48:45 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Wed, 19 Aug 2020 22:48:45 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Wed, 19 Aug 2020 22:48:45 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Wed, 19 Aug 2020 22:48:46 GMT
ARG OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:48:46 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.3
# Wed, 19 Aug 2020 22:48:46 GMT
COPY dir:db13e0b286891a0bd7aa45ab6285056101f78bde154aff1711d0e2933840a07f in /opt/ol/helpers 
# Wed, 19 Aug 2020 22:48:46 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 19 Aug 2020 22:48:59 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 19 Aug 2020 22:49:03 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:49:05 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 19 Aug 2020 22:49:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 19 Aug 2020 22:49:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 19 Aug 2020 22:49:19 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 19 Aug 2020 22:49:19 GMT
USER 1001
# Wed, 19 Aug 2020 22:49:19 GMT
EXPOSE 9080 9443
# Wed, 19 Aug 2020 22:49:19 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 19 Aug 2020 22:49:20 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172b17642c4976ab19fd089c118bc5daf377f3a385fee3563d8af19598f2050`  
		Last Modified: Wed, 19 Aug 2020 22:05:35 GMT  
		Size: 48.4 MB (48386872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dfa59a43319950ed2738e122529b6b034f798a23077257b0cd1910c40ad574`  
		Last Modified: Wed, 19 Aug 2020 22:50:24 GMT  
		Size: 6.5 KB (6546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8e400b4e985535532b056a643b9ad936a4a2086931734bb02d805f47c0c30c`  
		Last Modified: Wed, 19 Aug 2020 22:50:22 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93bf828038129ec93ba11d0e72783ee2bd2cb09a01f68f92b77abf3abf5fe57`  
		Last Modified: Wed, 19 Aug 2020 22:50:30 GMT  
		Size: 155.1 MB (155084736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fe00d8b21f6d682fb115b5212b386cea20648d1425fd89d94b579a8589a7a0`  
		Last Modified: Wed, 19 Aug 2020 22:50:22 GMT  
		Size: 996.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06ed7665c9f16ef89267c846bcd994f7c0ae50c035437755b0796cc863ab214`  
		Last Modified: Wed, 19 Aug 2020 22:50:22 GMT  
		Size: 7.6 KB (7636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14ac1b48233f0cf20171e3550091564791a1a6ee50181f5a3f317a70745303b`  
		Last Modified: Wed, 19 Aug 2020 22:50:23 GMT  
		Size: 8.1 MB (8132510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.6-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:be3cde6d9e73464e817d76bd6eb3a718e91f66dd2d4ac34529513326855b0c67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.6-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:0b99a14b161879bfcefb8b0980d5f5aa5e6981016a82709737eb659390dee9ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.2 MB (272171664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a7a27642ac6abe9b55705583972cb4abacf0529e182cdac33e9b3d5ba2587e`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:00:38 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 02:18:08 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Thu, 20 Aug 2020 02:18:08 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Thu, 20 Aug 2020 02:18:08 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Thu, 20 Aug 2020 02:18:08 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Thu, 20 Aug 2020 02:18:08 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:18:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Thu, 20 Aug 2020 02:18:09 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 02:18:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 02:18:21 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 02:18:21 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:18:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 02:18:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 02:18:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 02:18:43 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 02:18:43 GMT
USER 1001
# Thu, 20 Aug 2020 02:18:44 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 02:18:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 02:18:44 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 02:18:49 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Thu, 20 Aug 2020 02:19:23 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a8737f865890826d26efd4c158416bd1188e715c783fd41548e040ef975dbe`  
		Last Modified: Wed, 19 Aug 2020 22:05:50 GMT  
		Size: 48.7 MB (48691306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee39c4a818ab74b3d4b8933953ed0e3c5016d9893d585ec70ca831b0203a5fc`  
		Last Modified: Thu, 20 Aug 2020 02:20:48 GMT  
		Size: 8.4 KB (8353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302aed9941b82ae3ab3817ecf284683e73865f098464c51cfb9a2320074033a6`  
		Last Modified: Thu, 20 Aug 2020 02:20:47 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a311799848d57a7f67ecc62cd376ab4c2cba79b7f17f9364e181476574ad89`  
		Last Modified: Thu, 20 Aug 2020 02:20:58 GMT  
		Size: 157.8 MB (157758945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1114286cbc2b0217d4f6e0e51056b40359816828a5c489df8ce2287ed726ba8a`  
		Last Modified: Thu, 20 Aug 2020 02:20:47 GMT  
		Size: 906.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fae59aa9ad3774fca6872d377da0caaa926a6096addc53411ad7c97b6ef972`  
		Last Modified: Thu, 20 Aug 2020 02:20:47 GMT  
		Size: 9.4 KB (9398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e57259be319f1df28ce52f26dd3405d1e0227072e2bac92f3f2263a0936be74`  
		Last Modified: Thu, 20 Aug 2020 02:20:48 GMT  
		Size: 8.2 MB (8249751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43da0160de1da2475d4df8ee3ed50d1e9391fcea950e6f21ef8ab94b0f5ab2fb`  
		Last Modified: Thu, 20 Aug 2020 02:21:01 GMT  
		Size: 963.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8852c30ac650215d27937484c47f7dd8fcaa2f4ff6e4d0d03fbb0a76a42339ab`  
		Last Modified: Thu, 20 Aug 2020 02:21:04 GMT  
		Size: 16.8 MB (16840138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.6-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:7e9e7151310dc7bb02eb28ccd26e30b92e11ac1435a0d061b244e8217d43e316
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.3 MB (273349680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8899ade9025949d4aa7a16564c22e3ec46b8b93012b530e244be0ea7183a94ae`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:33 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:33:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:33:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:33:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 03:18:17 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Thu, 20 Aug 2020 03:18:32 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Thu, 20 Aug 2020 03:18:39 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Thu, 20 Aug 2020 03:18:43 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Thu, 20 Aug 2020 03:18:47 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:18:52 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Thu, 20 Aug 2020 03:18:54 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 03:18:57 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 03:19:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 03:19:56 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:20:10 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 03:20:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 03:20:59 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 03:21:06 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 03:21:11 GMT
USER 1001
# Thu, 20 Aug 2020 03:21:18 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 03:21:23 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 03:21:27 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 03:21:51 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Thu, 20 Aug 2020 03:22:41 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59a1586230e65d6fbe8aebe774b944895c099ea81decb8818ba03aa8180880`  
		Last Modified: Wed, 19 Aug 2020 22:46:13 GMT  
		Size: 49.2 MB (49150099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008e72d201e080e71fae93889c2830e14ad9a7417bd1a54a5868022c2e426011`  
		Last Modified: Thu, 20 Aug 2020 03:26:56 GMT  
		Size: 8.4 KB (8384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e91258a9dad24f960f17ee5dcba0f2af1d078c7ce454bb14df3ec3a2338833c`  
		Last Modified: Thu, 20 Aug 2020 03:26:52 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c421042f87d5d94b0869e65cfe09ad3d657902105bc641db9ee5d9cc96bf75`  
		Last Modified: Thu, 20 Aug 2020 03:27:06 GMT  
		Size: 157.8 MB (157759323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a5089de6fd61bedf5fa390828c5f753105dda367c4924f71b31517fc304550`  
		Last Modified: Thu, 20 Aug 2020 03:26:51 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffb60ba82632b7a9188f71b9b6d336a486bb9d210607189bba71a125a08fccf`  
		Last Modified: Thu, 20 Aug 2020 03:26:51 GMT  
		Size: 9.5 KB (9520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccdaca27deb036e80f010b1ffda07b088c5e52a31c61cd42ad62f771d5e3049`  
		Last Modified: Thu, 20 Aug 2020 03:26:56 GMT  
		Size: 6.9 MB (6853790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde969756522bbeb301b35b9be1f214028e7cfb7d0164bea89351e7a7cbfdf0b`  
		Last Modified: Thu, 20 Aug 2020 03:27:17 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681ff666db6654899094f5e6d9bbd6be06c7f6f80d4981ece38d7b63b89122d3`  
		Last Modified: Thu, 20 Aug 2020 03:27:20 GMT  
		Size: 14.6 MB (14602429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.6-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:2df7f080bfafed3aa054cf49168e2e6dbc0e3cd93db59c4a768ca213adb8ba1d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.9 MB (268922005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d9446f117290714fb67b191a9c8e7b99cfc893c9b3e59597421541baaa8149`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:22 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 21:59:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:47:32 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Wed, 19 Aug 2020 22:47:32 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Wed, 19 Aug 2020 22:47:32 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Wed, 19 Aug 2020 22:47:33 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Wed, 19 Aug 2020 22:47:33 GMT
ARG OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:47:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Wed, 19 Aug 2020 22:47:33 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Wed, 19 Aug 2020 22:47:33 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 19 Aug 2020 22:47:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 19 Aug 2020 22:47:50 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:47:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 19 Aug 2020 22:47:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 19 Aug 2020 22:48:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 19 Aug 2020 22:48:05 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 19 Aug 2020 22:48:05 GMT
USER 1001
# Wed, 19 Aug 2020 22:48:05 GMT
EXPOSE 9080 9443
# Wed, 19 Aug 2020 22:48:05 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 19 Aug 2020 22:48:06 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Wed, 19 Aug 2020 22:48:14 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Wed, 19 Aug 2020 22:48:39 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172b17642c4976ab19fd089c118bc5daf377f3a385fee3563d8af19598f2050`  
		Last Modified: Wed, 19 Aug 2020 22:05:35 GMT  
		Size: 48.4 MB (48386872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999f5582a6091bbc64ca758579549f06ac1e4f1233697fad6aa854c1be704a2e`  
		Last Modified: Wed, 19 Aug 2020 22:50:04 GMT  
		Size: 8.4 KB (8383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ac5b9f03880f85550c18252fb795a8c3d590e8ee4aea70c1c7c4a5d496d5cc`  
		Last Modified: Wed, 19 Aug 2020 22:50:03 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35351e01fab383b7f296ea28907dbeded71210b4dabe330e0cd80fe927d6a98f`  
		Last Modified: Wed, 19 Aug 2020 22:50:10 GMT  
		Size: 157.8 MB (157758450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b1d0d78ab7990d79b86eccfc9d82f38d2b9ff87dda3590e1058cd61bd04fd0`  
		Last Modified: Wed, 19 Aug 2020 22:50:03 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8ba097e048198e8b001edf7f6acdfb37b4de48b8ee97e0152a14989e31e9a7`  
		Last Modified: Wed, 19 Aug 2020 22:50:02 GMT  
		Size: 9.5 KB (9496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e55fcc8299fec35f7cf7f2b8ff4f896671f36b2aecc90fe32277a02425ac8b`  
		Last Modified: Wed, 19 Aug 2020 22:50:03 GMT  
		Size: 7.4 MB (7449132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b76f11f35b47910bee307a40c7312d7c9a43b705c8bbe5f082f37f2c767d427`  
		Last Modified: Wed, 19 Aug 2020 22:50:15 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b99169b0a69641fc75dd1c54190b09b6428b9066ea5d92c2ed8b3ce8277575`  
		Last Modified: Wed, 19 Aug 2020 22:50:17 GMT  
		Size: 16.3 MB (16303495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.6-kernel-java8-openj9`

```console
$ docker pull open-liberty@sha256:5a2dc693a23c326e94978b79a482d41ac88fd5003d8d0fc7b19dbd851bda214a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.6-kernel-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:28857d9206a249e5198ef012d51eddf754c642a22e39dca8878c1186e60e0b7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.3 MB (255330563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50e7c2fef59c283ef788ba1a238e276c40aa0bc037ae2a58d6a7cbf6818a08ad`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:00:38 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 02:18:08 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Thu, 20 Aug 2020 02:18:08 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Thu, 20 Aug 2020 02:18:08 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Thu, 20 Aug 2020 02:18:08 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Thu, 20 Aug 2020 02:18:08 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:18:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Thu, 20 Aug 2020 02:18:09 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 02:18:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 02:18:21 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 02:18:21 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:18:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 02:18:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 02:18:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 02:18:43 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 02:18:43 GMT
USER 1001
# Thu, 20 Aug 2020 02:18:44 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 02:18:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 02:18:44 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a8737f865890826d26efd4c158416bd1188e715c783fd41548e040ef975dbe`  
		Last Modified: Wed, 19 Aug 2020 22:05:50 GMT  
		Size: 48.7 MB (48691306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee39c4a818ab74b3d4b8933953ed0e3c5016d9893d585ec70ca831b0203a5fc`  
		Last Modified: Thu, 20 Aug 2020 02:20:48 GMT  
		Size: 8.4 KB (8353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302aed9941b82ae3ab3817ecf284683e73865f098464c51cfb9a2320074033a6`  
		Last Modified: Thu, 20 Aug 2020 02:20:47 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a311799848d57a7f67ecc62cd376ab4c2cba79b7f17f9364e181476574ad89`  
		Last Modified: Thu, 20 Aug 2020 02:20:58 GMT  
		Size: 157.8 MB (157758945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1114286cbc2b0217d4f6e0e51056b40359816828a5c489df8ce2287ed726ba8a`  
		Last Modified: Thu, 20 Aug 2020 02:20:47 GMT  
		Size: 906.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fae59aa9ad3774fca6872d377da0caaa926a6096addc53411ad7c97b6ef972`  
		Last Modified: Thu, 20 Aug 2020 02:20:47 GMT  
		Size: 9.4 KB (9398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e57259be319f1df28ce52f26dd3405d1e0227072e2bac92f3f2263a0936be74`  
		Last Modified: Thu, 20 Aug 2020 02:20:48 GMT  
		Size: 8.2 MB (8249751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.6-kernel-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:89f590009c26248f70c113e67ffe6f8611ffec1251530ee7cd02815642a8c48e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.7 MB (258746284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:441f888ef0fa47294da239fa794d00b3403eb250f7d39de043961663fa00d3e6`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:33 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:33:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:33:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:33:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 03:18:17 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Thu, 20 Aug 2020 03:18:32 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Thu, 20 Aug 2020 03:18:39 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Thu, 20 Aug 2020 03:18:43 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Thu, 20 Aug 2020 03:18:47 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:18:52 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Thu, 20 Aug 2020 03:18:54 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 03:18:57 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 03:19:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 03:19:56 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:20:10 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 03:20:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 03:20:59 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 03:21:06 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 03:21:11 GMT
USER 1001
# Thu, 20 Aug 2020 03:21:18 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 03:21:23 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 03:21:27 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59a1586230e65d6fbe8aebe774b944895c099ea81decb8818ba03aa8180880`  
		Last Modified: Wed, 19 Aug 2020 22:46:13 GMT  
		Size: 49.2 MB (49150099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008e72d201e080e71fae93889c2830e14ad9a7417bd1a54a5868022c2e426011`  
		Last Modified: Thu, 20 Aug 2020 03:26:56 GMT  
		Size: 8.4 KB (8384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e91258a9dad24f960f17ee5dcba0f2af1d078c7ce454bb14df3ec3a2338833c`  
		Last Modified: Thu, 20 Aug 2020 03:26:52 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c421042f87d5d94b0869e65cfe09ad3d657902105bc641db9ee5d9cc96bf75`  
		Last Modified: Thu, 20 Aug 2020 03:27:06 GMT  
		Size: 157.8 MB (157759323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a5089de6fd61bedf5fa390828c5f753105dda367c4924f71b31517fc304550`  
		Last Modified: Thu, 20 Aug 2020 03:26:51 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffb60ba82632b7a9188f71b9b6d336a486bb9d210607189bba71a125a08fccf`  
		Last Modified: Thu, 20 Aug 2020 03:26:51 GMT  
		Size: 9.5 KB (9520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccdaca27deb036e80f010b1ffda07b088c5e52a31c61cd42ad62f771d5e3049`  
		Last Modified: Thu, 20 Aug 2020 03:26:56 GMT  
		Size: 6.9 MB (6853790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.6-kernel-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:0f5a4edfc7cd654db55d4fa2f78a8e12ceae1aceb6a6054dabf5bf7bed4d5355
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.6 MB (252617546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee70cb2be70ab90a67dbbb0694ea19b034fcefd6b70a1d7a4413ff457dd1aa7f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:22 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 21:59:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:47:32 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Wed, 19 Aug 2020 22:47:32 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Wed, 19 Aug 2020 22:47:32 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Wed, 19 Aug 2020 22:47:33 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Wed, 19 Aug 2020 22:47:33 GMT
ARG OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:47:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Wed, 19 Aug 2020 22:47:33 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Wed, 19 Aug 2020 22:47:33 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 19 Aug 2020 22:47:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 19 Aug 2020 22:47:50 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:47:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 19 Aug 2020 22:47:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 19 Aug 2020 22:48:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 19 Aug 2020 22:48:05 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 19 Aug 2020 22:48:05 GMT
USER 1001
# Wed, 19 Aug 2020 22:48:05 GMT
EXPOSE 9080 9443
# Wed, 19 Aug 2020 22:48:05 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 19 Aug 2020 22:48:06 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172b17642c4976ab19fd089c118bc5daf377f3a385fee3563d8af19598f2050`  
		Last Modified: Wed, 19 Aug 2020 22:05:35 GMT  
		Size: 48.4 MB (48386872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999f5582a6091bbc64ca758579549f06ac1e4f1233697fad6aa854c1be704a2e`  
		Last Modified: Wed, 19 Aug 2020 22:50:04 GMT  
		Size: 8.4 KB (8383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ac5b9f03880f85550c18252fb795a8c3d590e8ee4aea70c1c7c4a5d496d5cc`  
		Last Modified: Wed, 19 Aug 2020 22:50:03 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35351e01fab383b7f296ea28907dbeded71210b4dabe330e0cd80fe927d6a98f`  
		Last Modified: Wed, 19 Aug 2020 22:50:10 GMT  
		Size: 157.8 MB (157758450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b1d0d78ab7990d79b86eccfc9d82f38d2b9ff87dda3590e1058cd61bd04fd0`  
		Last Modified: Wed, 19 Aug 2020 22:50:03 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8ba097e048198e8b001edf7f6acdfb37b4de48b8ee97e0152a14989e31e9a7`  
		Last Modified: Wed, 19 Aug 2020 22:50:02 GMT  
		Size: 9.5 KB (9496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e55fcc8299fec35f7cf7f2b8ff4f896671f36b2aecc90fe32277a02425ac8b`  
		Last Modified: Wed, 19 Aug 2020 22:50:03 GMT  
		Size: 7.4 MB (7449132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.8-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:653bc5b94658baf23fad2f69e91477a95ec86c0db9f738763a825107882c413d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.8-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:7cbe0cfd4556d2484c1f7054179541681d9b31a76f72086b9fe77869990082ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.2 MB (272154665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02d04f1ae31520d1f366a0ed0fa838952d13c24556a0460f8cd411523e83344d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:00:38 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 02:16:32 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:32 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 02:16:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 02:16:44 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 02:16:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 02:17:07 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 02:17:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 02:17:08 GMT
USER 1001
# Thu, 20 Aug 2020 02:17:08 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 02:17:08 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 02:17:08 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 02:17:21 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Thu, 20 Aug 2020 02:17:55 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a8737f865890826d26efd4c158416bd1188e715c783fd41548e040ef975dbe`  
		Last Modified: Wed, 19 Aug 2020 22:05:50 GMT  
		Size: 48.7 MB (48691306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6597d5c2fcc114d8288a0802f34d16d564cb007ed2d59d38188aa091be14b25d`  
		Last Modified: Thu, 20 Aug 2020 02:20:24 GMT  
		Size: 8.4 KB (8352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888430f050ceadc370b33895dc685299bfd5a255de3160addf3e8887d57ad3c1`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34bb89999af5eea4a3a2270b33aab65b156ded317b60b50da02b17e14762d37`  
		Last Modified: Thu, 20 Aug 2020 02:20:34 GMT  
		Size: 157.8 MB (157847581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea7686ef22dccde6374800a0a8af564aab1d2ce37971d5491effba12f260f83`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd604c0109bce96a7f35816d7a30c902b84f8cafc5121ae095a6e3bb00b07fc4`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 9.4 KB (9400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6cc4e7ae36550db2126f74e99c81b6d5eb44b5f5b38112ff7272b531c91db`  
		Last Modified: Thu, 20 Aug 2020 02:20:25 GMT  
		Size: 8.1 MB (8057281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996a7ba33d6ba87063fb63dd6b87d739a5c0ebae06b7ac2867d34a17af16c0a3`  
		Last Modified: Thu, 20 Aug 2020 02:20:38 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3fd1c9f3fd3f9472a9dddda0b74f0edf7b5ae82f7d7bf7fb104c3e63bd634d`  
		Last Modified: Thu, 20 Aug 2020 02:20:41 GMT  
		Size: 16.9 MB (16926973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.8-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:cfc22d235e304fb21276e202255d52b979ce40e105a1ab420fd1f17418abcca4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.6 MB (273578130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7be0bb5cbe3179d1a1d907492325e9237827a8a8f805ab37c1b5788f12975fe8`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:33 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:33:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:33:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:33:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 03:13:43 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 03:13:46 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 03:13:49 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 03:13:52 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 03:13:53 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:14:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 03:14:02 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 03:14:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 03:14:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 03:15:06 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:15:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 03:15:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 03:16:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 03:16:09 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 03:16:12 GMT
USER 1001
# Thu, 20 Aug 2020 03:16:18 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 03:16:23 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 03:16:29 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 03:16:49 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Thu, 20 Aug 2020 03:17:48 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59a1586230e65d6fbe8aebe774b944895c099ea81decb8818ba03aa8180880`  
		Last Modified: Wed, 19 Aug 2020 22:46:13 GMT  
		Size: 49.2 MB (49150099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ec4d988366d9ca7186bc54ce46603179ccf0681f888dc0d42e8cb0c3e7d01d`  
		Last Modified: Thu, 20 Aug 2020 03:26:08 GMT  
		Size: 8.4 KB (8383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1de4b8fd3a1677f86db2f581b69d6b8ec280d723044406d5873ef487e619738`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a445138c34d32647f9b4d494a0fa8d79332a812060b2c8ff31ef187339c1e9e`  
		Last Modified: Thu, 20 Aug 2020 03:26:17 GMT  
		Size: 157.8 MB (157848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6f8ed2c43944590fd32a48b0d2074618a6245b71a2ed18462d5c96e676b6c`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa47e1e197708807cfe4e1f6eae85c6097ceb9ff78de264cd77ff350acb85f`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 9.5 KB (9523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d2059ad7e51f9f633a992795b9d65cee7c9666fc49ff54680de2ce3ea9383`  
		Last Modified: Thu, 20 Aug 2020 03:26:05 GMT  
		Size: 6.9 MB (6918933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99121a436a07f2e84c54768e407a35724fb9a63574e29822e45ddcbde16aeb44`  
		Last Modified: Thu, 20 Aug 2020 03:26:29 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4d071db851d85c4d43f702c7b21e45077482c290f5d9fdb4f0be564a861dda`  
		Last Modified: Thu, 20 Aug 2020 03:26:33 GMT  
		Size: 14.7 MB (14676987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.8-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:842c5646b1c1e6d9b3a2aabd4883f4bcbf1c92690eb23cb7e874c6bf02bc1df2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.0 MB (269026630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c069ce61a624fb5ddfc3281f89c87b994492debae51d4aed6fa84b1c88d34f77`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:22 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 21:59:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Wed, 19 Aug 2020 22:46:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Wed, 19 Aug 2020 22:46:12 GMT
ARG OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 19 Aug 2020 22:46:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 19 Aug 2020 22:46:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 19 Aug 2020 22:46:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 19 Aug 2020 22:46:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 19 Aug 2020 22:46:44 GMT
USER 1001
# Wed, 19 Aug 2020 22:46:44 GMT
EXPOSE 9080 9443
# Wed, 19 Aug 2020 22:46:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 19 Aug 2020 22:46:45 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Wed, 19 Aug 2020 22:46:53 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Wed, 19 Aug 2020 22:47:16 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172b17642c4976ab19fd089c118bc5daf377f3a385fee3563d8af19598f2050`  
		Last Modified: Wed, 19 Aug 2020 22:05:35 GMT  
		Size: 48.4 MB (48386872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b611fd8ca23c160b4762d74a71c9cd634b4be59334c057b753ef115bae4fa3`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f6082ead0ee7fd5c965e9518845d895223681b0c395081b672e61f8609caae`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779a45a76e45c81bb2bd668adcc03deb55d44c66a727d5a5d873453a026b0b50`  
		Last Modified: Wed, 19 Aug 2020 22:49:45 GMT  
		Size: 157.8 MB (157847156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccc2d7faf8eb3abf7b4ce036697fd93cd747f4a743925d3bb2e15ac5f87983b`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadd59fcc56ef3a1cf58e38625ca4ea1cb83c64dfb48bed436b55ad040c19ce8`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 9.5 KB (9495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5f8433ef858963b930e4ebb8360bf2fdb8d5eb829dac045a68b0ca29230d38`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 7.5 MB (7491626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6810ce5a1c4bc7a1c60c6f4d422dbcf2fe75f9ec78f516ee244c874f98b56836`  
		Last Modified: Wed, 19 Aug 2020 22:49:51 GMT  
		Size: 965.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e59c06f29d6550fa79ae98c6540ed99bf540e00af155ff14140df006a62e3f`  
		Last Modified: Wed, 19 Aug 2020 22:49:53 GMT  
		Size: 16.3 MB (16276917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.8-kernel-java8-openj9`

```console
$ docker pull open-liberty@sha256:fd97fdb746c0db30d67ab46844614ada2a393b84f06ac00b471f3c97d5d00afd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.8-kernel-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:a4313f5b0c4c2a8e5a31229c4c3382e8dd1594ce56c0b1b38c9946e00c176104
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255226732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a79b631432e59abdf58b5bdf4708404ed3c944dcaab13aa82916d3a05824dc1f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:00:38 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 02:16:32 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:32 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 02:16:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 02:16:44 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 02:16:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 02:17:07 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 02:17:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 02:17:08 GMT
USER 1001
# Thu, 20 Aug 2020 02:17:08 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 02:17:08 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 02:17:08 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a8737f865890826d26efd4c158416bd1188e715c783fd41548e040ef975dbe`  
		Last Modified: Wed, 19 Aug 2020 22:05:50 GMT  
		Size: 48.7 MB (48691306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6597d5c2fcc114d8288a0802f34d16d564cb007ed2d59d38188aa091be14b25d`  
		Last Modified: Thu, 20 Aug 2020 02:20:24 GMT  
		Size: 8.4 KB (8352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888430f050ceadc370b33895dc685299bfd5a255de3160addf3e8887d57ad3c1`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34bb89999af5eea4a3a2270b33aab65b156ded317b60b50da02b17e14762d37`  
		Last Modified: Thu, 20 Aug 2020 02:20:34 GMT  
		Size: 157.8 MB (157847581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea7686ef22dccde6374800a0a8af564aab1d2ce37971d5491effba12f260f83`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd604c0109bce96a7f35816d7a30c902b84f8cafc5121ae095a6e3bb00b07fc4`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 9.4 KB (9400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6cc4e7ae36550db2126f74e99c81b6d5eb44b5f5b38112ff7272b531c91db`  
		Last Modified: Thu, 20 Aug 2020 02:20:25 GMT  
		Size: 8.1 MB (8057281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.8-kernel-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:b174fb6ecc4aa57b1854a757803017cc2a80d52024db88003087454a4816caee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.9 MB (258900177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e2a702674a028f07a04d7746be0d2b8fd522504d4841fc49119c6c1229e9f19`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:33 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:33:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:33:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:33:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 03:13:43 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 03:13:46 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 03:13:49 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 03:13:52 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 03:13:53 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:14:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 03:14:02 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 03:14:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 03:14:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 03:15:06 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:15:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 03:15:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 03:16:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 03:16:09 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 03:16:12 GMT
USER 1001
# Thu, 20 Aug 2020 03:16:18 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 03:16:23 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 03:16:29 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59a1586230e65d6fbe8aebe774b944895c099ea81decb8818ba03aa8180880`  
		Last Modified: Wed, 19 Aug 2020 22:46:13 GMT  
		Size: 49.2 MB (49150099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ec4d988366d9ca7186bc54ce46603179ccf0681f888dc0d42e8cb0c3e7d01d`  
		Last Modified: Thu, 20 Aug 2020 03:26:08 GMT  
		Size: 8.4 KB (8383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1de4b8fd3a1677f86db2f581b69d6b8ec280d723044406d5873ef487e619738`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a445138c34d32647f9b4d494a0fa8d79332a812060b2c8ff31ef187339c1e9e`  
		Last Modified: Thu, 20 Aug 2020 03:26:17 GMT  
		Size: 157.8 MB (157848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6f8ed2c43944590fd32a48b0d2074618a6245b71a2ed18462d5c96e676b6c`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa47e1e197708807cfe4e1f6eae85c6097ceb9ff78de264cd77ff350acb85f`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 9.5 KB (9523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d2059ad7e51f9f633a992795b9d65cee7c9666fc49ff54680de2ce3ea9383`  
		Last Modified: Thu, 20 Aug 2020 03:26:05 GMT  
		Size: 6.9 MB (6918933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.8-kernel-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:05bf5c4a2fa8306879d1a6a2df12cb425b6ae3523cea0ab1dbd494cdcfcf7af7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.7 MB (252748748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9f068c4d4dae36f005eed0b5bc6797995229b69d3f46fcba867e03479aa2f0a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:22 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 21:59:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Wed, 19 Aug 2020 22:46:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Wed, 19 Aug 2020 22:46:12 GMT
ARG OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 19 Aug 2020 22:46:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 19 Aug 2020 22:46:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 19 Aug 2020 22:46:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 19 Aug 2020 22:46:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 19 Aug 2020 22:46:44 GMT
USER 1001
# Wed, 19 Aug 2020 22:46:44 GMT
EXPOSE 9080 9443
# Wed, 19 Aug 2020 22:46:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 19 Aug 2020 22:46:45 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172b17642c4976ab19fd089c118bc5daf377f3a385fee3563d8af19598f2050`  
		Last Modified: Wed, 19 Aug 2020 22:05:35 GMT  
		Size: 48.4 MB (48386872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b611fd8ca23c160b4762d74a71c9cd634b4be59334c057b753ef115bae4fa3`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f6082ead0ee7fd5c965e9518845d895223681b0c395081b672e61f8609caae`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779a45a76e45c81bb2bd668adcc03deb55d44c66a727d5a5d873453a026b0b50`  
		Last Modified: Wed, 19 Aug 2020 22:49:45 GMT  
		Size: 157.8 MB (157847156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccc2d7faf8eb3abf7b4ce036697fd93cd747f4a743925d3bb2e15ac5f87983b`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadd59fcc56ef3a1cf58e38625ca4ea1cb83c64dfb48bed436b55ad040c19ce8`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 9.5 KB (9495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5f8433ef858963b930e4ebb8360bf2fdb8d5eb829dac045a68b0ca29230d38`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 7.5 MB (7491626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:full`

```console
$ docker pull open-liberty@sha256:653bc5b94658baf23fad2f69e91477a95ec86c0db9f738763a825107882c413d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full` - linux; amd64

```console
$ docker pull open-liberty@sha256:7cbe0cfd4556d2484c1f7054179541681d9b31a76f72086b9fe77869990082ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.2 MB (272154665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02d04f1ae31520d1f366a0ed0fa838952d13c24556a0460f8cd411523e83344d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:00:38 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 02:16:32 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:32 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 02:16:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 02:16:44 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 02:16:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 02:17:07 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 02:17:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 02:17:08 GMT
USER 1001
# Thu, 20 Aug 2020 02:17:08 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 02:17:08 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 02:17:08 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 02:17:21 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Thu, 20 Aug 2020 02:17:55 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a8737f865890826d26efd4c158416bd1188e715c783fd41548e040ef975dbe`  
		Last Modified: Wed, 19 Aug 2020 22:05:50 GMT  
		Size: 48.7 MB (48691306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6597d5c2fcc114d8288a0802f34d16d564cb007ed2d59d38188aa091be14b25d`  
		Last Modified: Thu, 20 Aug 2020 02:20:24 GMT  
		Size: 8.4 KB (8352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888430f050ceadc370b33895dc685299bfd5a255de3160addf3e8887d57ad3c1`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34bb89999af5eea4a3a2270b33aab65b156ded317b60b50da02b17e14762d37`  
		Last Modified: Thu, 20 Aug 2020 02:20:34 GMT  
		Size: 157.8 MB (157847581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea7686ef22dccde6374800a0a8af564aab1d2ce37971d5491effba12f260f83`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd604c0109bce96a7f35816d7a30c902b84f8cafc5121ae095a6e3bb00b07fc4`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 9.4 KB (9400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6cc4e7ae36550db2126f74e99c81b6d5eb44b5f5b38112ff7272b531c91db`  
		Last Modified: Thu, 20 Aug 2020 02:20:25 GMT  
		Size: 8.1 MB (8057281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996a7ba33d6ba87063fb63dd6b87d739a5c0ebae06b7ac2867d34a17af16c0a3`  
		Last Modified: Thu, 20 Aug 2020 02:20:38 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3fd1c9f3fd3f9472a9dddda0b74f0edf7b5ae82f7d7bf7fb104c3e63bd634d`  
		Last Modified: Thu, 20 Aug 2020 02:20:41 GMT  
		Size: 16.9 MB (16926973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:cfc22d235e304fb21276e202255d52b979ce40e105a1ab420fd1f17418abcca4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.6 MB (273578130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7be0bb5cbe3179d1a1d907492325e9237827a8a8f805ab37c1b5788f12975fe8`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:33 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:33:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:33:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:33:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 03:13:43 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 03:13:46 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 03:13:49 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 03:13:52 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 03:13:53 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:14:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 03:14:02 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 03:14:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 03:14:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 03:15:06 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:15:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 03:15:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 03:16:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 03:16:09 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 03:16:12 GMT
USER 1001
# Thu, 20 Aug 2020 03:16:18 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 03:16:23 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 03:16:29 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 03:16:49 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Thu, 20 Aug 2020 03:17:48 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59a1586230e65d6fbe8aebe774b944895c099ea81decb8818ba03aa8180880`  
		Last Modified: Wed, 19 Aug 2020 22:46:13 GMT  
		Size: 49.2 MB (49150099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ec4d988366d9ca7186bc54ce46603179ccf0681f888dc0d42e8cb0c3e7d01d`  
		Last Modified: Thu, 20 Aug 2020 03:26:08 GMT  
		Size: 8.4 KB (8383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1de4b8fd3a1677f86db2f581b69d6b8ec280d723044406d5873ef487e619738`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a445138c34d32647f9b4d494a0fa8d79332a812060b2c8ff31ef187339c1e9e`  
		Last Modified: Thu, 20 Aug 2020 03:26:17 GMT  
		Size: 157.8 MB (157848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6f8ed2c43944590fd32a48b0d2074618a6245b71a2ed18462d5c96e676b6c`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa47e1e197708807cfe4e1f6eae85c6097ceb9ff78de264cd77ff350acb85f`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 9.5 KB (9523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d2059ad7e51f9f633a992795b9d65cee7c9666fc49ff54680de2ce3ea9383`  
		Last Modified: Thu, 20 Aug 2020 03:26:05 GMT  
		Size: 6.9 MB (6918933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99121a436a07f2e84c54768e407a35724fb9a63574e29822e45ddcbde16aeb44`  
		Last Modified: Thu, 20 Aug 2020 03:26:29 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4d071db851d85c4d43f702c7b21e45077482c290f5d9fdb4f0be564a861dda`  
		Last Modified: Thu, 20 Aug 2020 03:26:33 GMT  
		Size: 14.7 MB (14676987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; s390x

```console
$ docker pull open-liberty@sha256:842c5646b1c1e6d9b3a2aabd4883f4bcbf1c92690eb23cb7e874c6bf02bc1df2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.0 MB (269026630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c069ce61a624fb5ddfc3281f89c87b994492debae51d4aed6fa84b1c88d34f77`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:22 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 21:59:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Wed, 19 Aug 2020 22:46:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Wed, 19 Aug 2020 22:46:12 GMT
ARG OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 19 Aug 2020 22:46:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 19 Aug 2020 22:46:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 19 Aug 2020 22:46:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 19 Aug 2020 22:46:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 19 Aug 2020 22:46:44 GMT
USER 1001
# Wed, 19 Aug 2020 22:46:44 GMT
EXPOSE 9080 9443
# Wed, 19 Aug 2020 22:46:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 19 Aug 2020 22:46:45 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Wed, 19 Aug 2020 22:46:53 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Wed, 19 Aug 2020 22:47:16 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172b17642c4976ab19fd089c118bc5daf377f3a385fee3563d8af19598f2050`  
		Last Modified: Wed, 19 Aug 2020 22:05:35 GMT  
		Size: 48.4 MB (48386872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b611fd8ca23c160b4762d74a71c9cd634b4be59334c057b753ef115bae4fa3`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f6082ead0ee7fd5c965e9518845d895223681b0c395081b672e61f8609caae`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779a45a76e45c81bb2bd668adcc03deb55d44c66a727d5a5d873453a026b0b50`  
		Last Modified: Wed, 19 Aug 2020 22:49:45 GMT  
		Size: 157.8 MB (157847156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccc2d7faf8eb3abf7b4ce036697fd93cd747f4a743925d3bb2e15ac5f87983b`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadd59fcc56ef3a1cf58e38625ca4ea1cb83c64dfb48bed436b55ad040c19ce8`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 9.5 KB (9495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5f8433ef858963b930e4ebb8360bf2fdb8d5eb829dac045a68b0ca29230d38`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 7.5 MB (7491626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6810ce5a1c4bc7a1c60c6f4d422dbcf2fe75f9ec78f516ee244c874f98b56836`  
		Last Modified: Wed, 19 Aug 2020 22:49:51 GMT  
		Size: 965.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e59c06f29d6550fa79ae98c6540ed99bf540e00af155ff14140df006a62e3f`  
		Last Modified: Wed, 19 Aug 2020 22:49:53 GMT  
		Size: 16.3 MB (16276917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:full-java8-openj9`

```console
$ docker pull open-liberty@sha256:653bc5b94658baf23fad2f69e91477a95ec86c0db9f738763a825107882c413d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:7cbe0cfd4556d2484c1f7054179541681d9b31a76f72086b9fe77869990082ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.2 MB (272154665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02d04f1ae31520d1f366a0ed0fa838952d13c24556a0460f8cd411523e83344d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:00:38 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 02:16:32 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:32 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 02:16:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 02:16:44 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 02:16:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 02:17:07 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 02:17:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 02:17:08 GMT
USER 1001
# Thu, 20 Aug 2020 02:17:08 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 02:17:08 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 02:17:08 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 02:17:21 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Thu, 20 Aug 2020 02:17:55 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a8737f865890826d26efd4c158416bd1188e715c783fd41548e040ef975dbe`  
		Last Modified: Wed, 19 Aug 2020 22:05:50 GMT  
		Size: 48.7 MB (48691306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6597d5c2fcc114d8288a0802f34d16d564cb007ed2d59d38188aa091be14b25d`  
		Last Modified: Thu, 20 Aug 2020 02:20:24 GMT  
		Size: 8.4 KB (8352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888430f050ceadc370b33895dc685299bfd5a255de3160addf3e8887d57ad3c1`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34bb89999af5eea4a3a2270b33aab65b156ded317b60b50da02b17e14762d37`  
		Last Modified: Thu, 20 Aug 2020 02:20:34 GMT  
		Size: 157.8 MB (157847581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea7686ef22dccde6374800a0a8af564aab1d2ce37971d5491effba12f260f83`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd604c0109bce96a7f35816d7a30c902b84f8cafc5121ae095a6e3bb00b07fc4`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 9.4 KB (9400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6cc4e7ae36550db2126f74e99c81b6d5eb44b5f5b38112ff7272b531c91db`  
		Last Modified: Thu, 20 Aug 2020 02:20:25 GMT  
		Size: 8.1 MB (8057281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996a7ba33d6ba87063fb63dd6b87d739a5c0ebae06b7ac2867d34a17af16c0a3`  
		Last Modified: Thu, 20 Aug 2020 02:20:38 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3fd1c9f3fd3f9472a9dddda0b74f0edf7b5ae82f7d7bf7fb104c3e63bd634d`  
		Last Modified: Thu, 20 Aug 2020 02:20:41 GMT  
		Size: 16.9 MB (16926973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:cfc22d235e304fb21276e202255d52b979ce40e105a1ab420fd1f17418abcca4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.6 MB (273578130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7be0bb5cbe3179d1a1d907492325e9237827a8a8f805ab37c1b5788f12975fe8`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:33 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:33:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:33:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:33:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 03:13:43 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 03:13:46 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 03:13:49 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 03:13:52 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 03:13:53 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:14:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 03:14:02 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 03:14:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 03:14:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 03:15:06 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:15:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 03:15:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 03:16:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 03:16:09 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 03:16:12 GMT
USER 1001
# Thu, 20 Aug 2020 03:16:18 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 03:16:23 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 03:16:29 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 03:16:49 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Thu, 20 Aug 2020 03:17:48 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59a1586230e65d6fbe8aebe774b944895c099ea81decb8818ba03aa8180880`  
		Last Modified: Wed, 19 Aug 2020 22:46:13 GMT  
		Size: 49.2 MB (49150099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ec4d988366d9ca7186bc54ce46603179ccf0681f888dc0d42e8cb0c3e7d01d`  
		Last Modified: Thu, 20 Aug 2020 03:26:08 GMT  
		Size: 8.4 KB (8383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1de4b8fd3a1677f86db2f581b69d6b8ec280d723044406d5873ef487e619738`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a445138c34d32647f9b4d494a0fa8d79332a812060b2c8ff31ef187339c1e9e`  
		Last Modified: Thu, 20 Aug 2020 03:26:17 GMT  
		Size: 157.8 MB (157848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6f8ed2c43944590fd32a48b0d2074618a6245b71a2ed18462d5c96e676b6c`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa47e1e197708807cfe4e1f6eae85c6097ceb9ff78de264cd77ff350acb85f`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 9.5 KB (9523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d2059ad7e51f9f633a992795b9d65cee7c9666fc49ff54680de2ce3ea9383`  
		Last Modified: Thu, 20 Aug 2020 03:26:05 GMT  
		Size: 6.9 MB (6918933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99121a436a07f2e84c54768e407a35724fb9a63574e29822e45ddcbde16aeb44`  
		Last Modified: Thu, 20 Aug 2020 03:26:29 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4d071db851d85c4d43f702c7b21e45077482c290f5d9fdb4f0be564a861dda`  
		Last Modified: Thu, 20 Aug 2020 03:26:33 GMT  
		Size: 14.7 MB (14676987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:842c5646b1c1e6d9b3a2aabd4883f4bcbf1c92690eb23cb7e874c6bf02bc1df2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.0 MB (269026630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c069ce61a624fb5ddfc3281f89c87b994492debae51d4aed6fa84b1c88d34f77`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:22 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 21:59:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Wed, 19 Aug 2020 22:46:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Wed, 19 Aug 2020 22:46:12 GMT
ARG OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 19 Aug 2020 22:46:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 19 Aug 2020 22:46:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 19 Aug 2020 22:46:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 19 Aug 2020 22:46:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 19 Aug 2020 22:46:44 GMT
USER 1001
# Wed, 19 Aug 2020 22:46:44 GMT
EXPOSE 9080 9443
# Wed, 19 Aug 2020 22:46:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 19 Aug 2020 22:46:45 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Wed, 19 Aug 2020 22:46:53 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Wed, 19 Aug 2020 22:47:16 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172b17642c4976ab19fd089c118bc5daf377f3a385fee3563d8af19598f2050`  
		Last Modified: Wed, 19 Aug 2020 22:05:35 GMT  
		Size: 48.4 MB (48386872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b611fd8ca23c160b4762d74a71c9cd634b4be59334c057b753ef115bae4fa3`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f6082ead0ee7fd5c965e9518845d895223681b0c395081b672e61f8609caae`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779a45a76e45c81bb2bd668adcc03deb55d44c66a727d5a5d873453a026b0b50`  
		Last Modified: Wed, 19 Aug 2020 22:49:45 GMT  
		Size: 157.8 MB (157847156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccc2d7faf8eb3abf7b4ce036697fd93cd747f4a743925d3bb2e15ac5f87983b`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadd59fcc56ef3a1cf58e38625ca4ea1cb83c64dfb48bed436b55ad040c19ce8`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 9.5 KB (9495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5f8433ef858963b930e4ebb8360bf2fdb8d5eb829dac045a68b0ca29230d38`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 7.5 MB (7491626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6810ce5a1c4bc7a1c60c6f4d422dbcf2fe75f9ec78f516ee244c874f98b56836`  
		Last Modified: Wed, 19 Aug 2020 22:49:51 GMT  
		Size: 965.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e59c06f29d6550fa79ae98c6540ed99bf540e00af155ff14140df006a62e3f`  
		Last Modified: Wed, 19 Aug 2020 22:49:53 GMT  
		Size: 16.3 MB (16276917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:kernel`

```console
$ docker pull open-liberty@sha256:fd97fdb746c0db30d67ab46844614ada2a393b84f06ac00b471f3c97d5d00afd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel` - linux; amd64

```console
$ docker pull open-liberty@sha256:a4313f5b0c4c2a8e5a31229c4c3382e8dd1594ce56c0b1b38c9946e00c176104
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255226732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a79b631432e59abdf58b5bdf4708404ed3c944dcaab13aa82916d3a05824dc1f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:00:38 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 02:16:32 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:32 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 02:16:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 02:16:44 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 02:16:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 02:17:07 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 02:17:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 02:17:08 GMT
USER 1001
# Thu, 20 Aug 2020 02:17:08 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 02:17:08 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 02:17:08 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a8737f865890826d26efd4c158416bd1188e715c783fd41548e040ef975dbe`  
		Last Modified: Wed, 19 Aug 2020 22:05:50 GMT  
		Size: 48.7 MB (48691306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6597d5c2fcc114d8288a0802f34d16d564cb007ed2d59d38188aa091be14b25d`  
		Last Modified: Thu, 20 Aug 2020 02:20:24 GMT  
		Size: 8.4 KB (8352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888430f050ceadc370b33895dc685299bfd5a255de3160addf3e8887d57ad3c1`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34bb89999af5eea4a3a2270b33aab65b156ded317b60b50da02b17e14762d37`  
		Last Modified: Thu, 20 Aug 2020 02:20:34 GMT  
		Size: 157.8 MB (157847581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea7686ef22dccde6374800a0a8af564aab1d2ce37971d5491effba12f260f83`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd604c0109bce96a7f35816d7a30c902b84f8cafc5121ae095a6e3bb00b07fc4`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 9.4 KB (9400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6cc4e7ae36550db2126f74e99c81b6d5eb44b5f5b38112ff7272b531c91db`  
		Last Modified: Thu, 20 Aug 2020 02:20:25 GMT  
		Size: 8.1 MB (8057281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:b174fb6ecc4aa57b1854a757803017cc2a80d52024db88003087454a4816caee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.9 MB (258900177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e2a702674a028f07a04d7746be0d2b8fd522504d4841fc49119c6c1229e9f19`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:33 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:33:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:33:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:33:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 03:13:43 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 03:13:46 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 03:13:49 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 03:13:52 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 03:13:53 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:14:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 03:14:02 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 03:14:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 03:14:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 03:15:06 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:15:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 03:15:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 03:16:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 03:16:09 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 03:16:12 GMT
USER 1001
# Thu, 20 Aug 2020 03:16:18 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 03:16:23 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 03:16:29 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59a1586230e65d6fbe8aebe774b944895c099ea81decb8818ba03aa8180880`  
		Last Modified: Wed, 19 Aug 2020 22:46:13 GMT  
		Size: 49.2 MB (49150099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ec4d988366d9ca7186bc54ce46603179ccf0681f888dc0d42e8cb0c3e7d01d`  
		Last Modified: Thu, 20 Aug 2020 03:26:08 GMT  
		Size: 8.4 KB (8383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1de4b8fd3a1677f86db2f581b69d6b8ec280d723044406d5873ef487e619738`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a445138c34d32647f9b4d494a0fa8d79332a812060b2c8ff31ef187339c1e9e`  
		Last Modified: Thu, 20 Aug 2020 03:26:17 GMT  
		Size: 157.8 MB (157848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6f8ed2c43944590fd32a48b0d2074618a6245b71a2ed18462d5c96e676b6c`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa47e1e197708807cfe4e1f6eae85c6097ceb9ff78de264cd77ff350acb85f`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 9.5 KB (9523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d2059ad7e51f9f633a992795b9d65cee7c9666fc49ff54680de2ce3ea9383`  
		Last Modified: Thu, 20 Aug 2020 03:26:05 GMT  
		Size: 6.9 MB (6918933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel` - linux; s390x

```console
$ docker pull open-liberty@sha256:05bf5c4a2fa8306879d1a6a2df12cb425b6ae3523cea0ab1dbd494cdcfcf7af7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.7 MB (252748748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9f068c4d4dae36f005eed0b5bc6797995229b69d3f46fcba867e03479aa2f0a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:22 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 21:59:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Wed, 19 Aug 2020 22:46:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Wed, 19 Aug 2020 22:46:12 GMT
ARG OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 19 Aug 2020 22:46:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 19 Aug 2020 22:46:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 19 Aug 2020 22:46:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 19 Aug 2020 22:46:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 19 Aug 2020 22:46:44 GMT
USER 1001
# Wed, 19 Aug 2020 22:46:44 GMT
EXPOSE 9080 9443
# Wed, 19 Aug 2020 22:46:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 19 Aug 2020 22:46:45 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172b17642c4976ab19fd089c118bc5daf377f3a385fee3563d8af19598f2050`  
		Last Modified: Wed, 19 Aug 2020 22:05:35 GMT  
		Size: 48.4 MB (48386872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b611fd8ca23c160b4762d74a71c9cd634b4be59334c057b753ef115bae4fa3`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f6082ead0ee7fd5c965e9518845d895223681b0c395081b672e61f8609caae`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779a45a76e45c81bb2bd668adcc03deb55d44c66a727d5a5d873453a026b0b50`  
		Last Modified: Wed, 19 Aug 2020 22:49:45 GMT  
		Size: 157.8 MB (157847156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccc2d7faf8eb3abf7b4ce036697fd93cd747f4a743925d3bb2e15ac5f87983b`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadd59fcc56ef3a1cf58e38625ca4ea1cb83c64dfb48bed436b55ad040c19ce8`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 9.5 KB (9495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5f8433ef858963b930e4ebb8360bf2fdb8d5eb829dac045a68b0ca29230d38`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 7.5 MB (7491626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:kernel-java8-openj9`

```console
$ docker pull open-liberty@sha256:fd97fdb746c0db30d67ab46844614ada2a393b84f06ac00b471f3c97d5d00afd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:a4313f5b0c4c2a8e5a31229c4c3382e8dd1594ce56c0b1b38c9946e00c176104
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255226732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a79b631432e59abdf58b5bdf4708404ed3c944dcaab13aa82916d3a05824dc1f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:00:38 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 02:16:32 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:32 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 02:16:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 02:16:44 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 02:16:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 02:17:07 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 02:17:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 02:17:08 GMT
USER 1001
# Thu, 20 Aug 2020 02:17:08 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 02:17:08 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 02:17:08 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a8737f865890826d26efd4c158416bd1188e715c783fd41548e040ef975dbe`  
		Last Modified: Wed, 19 Aug 2020 22:05:50 GMT  
		Size: 48.7 MB (48691306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6597d5c2fcc114d8288a0802f34d16d564cb007ed2d59d38188aa091be14b25d`  
		Last Modified: Thu, 20 Aug 2020 02:20:24 GMT  
		Size: 8.4 KB (8352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888430f050ceadc370b33895dc685299bfd5a255de3160addf3e8887d57ad3c1`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34bb89999af5eea4a3a2270b33aab65b156ded317b60b50da02b17e14762d37`  
		Last Modified: Thu, 20 Aug 2020 02:20:34 GMT  
		Size: 157.8 MB (157847581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea7686ef22dccde6374800a0a8af564aab1d2ce37971d5491effba12f260f83`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd604c0109bce96a7f35816d7a30c902b84f8cafc5121ae095a6e3bb00b07fc4`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 9.4 KB (9400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6cc4e7ae36550db2126f74e99c81b6d5eb44b5f5b38112ff7272b531c91db`  
		Last Modified: Thu, 20 Aug 2020 02:20:25 GMT  
		Size: 8.1 MB (8057281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:b174fb6ecc4aa57b1854a757803017cc2a80d52024db88003087454a4816caee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.9 MB (258900177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e2a702674a028f07a04d7746be0d2b8fd522504d4841fc49119c6c1229e9f19`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:33 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:33:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:33:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:33:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 03:13:43 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 03:13:46 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 03:13:49 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 03:13:52 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 03:13:53 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:14:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 03:14:02 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 03:14:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 03:14:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 03:15:06 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:15:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 03:15:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 03:16:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 03:16:09 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 03:16:12 GMT
USER 1001
# Thu, 20 Aug 2020 03:16:18 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 03:16:23 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 03:16:29 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59a1586230e65d6fbe8aebe774b944895c099ea81decb8818ba03aa8180880`  
		Last Modified: Wed, 19 Aug 2020 22:46:13 GMT  
		Size: 49.2 MB (49150099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ec4d988366d9ca7186bc54ce46603179ccf0681f888dc0d42e8cb0c3e7d01d`  
		Last Modified: Thu, 20 Aug 2020 03:26:08 GMT  
		Size: 8.4 KB (8383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1de4b8fd3a1677f86db2f581b69d6b8ec280d723044406d5873ef487e619738`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a445138c34d32647f9b4d494a0fa8d79332a812060b2c8ff31ef187339c1e9e`  
		Last Modified: Thu, 20 Aug 2020 03:26:17 GMT  
		Size: 157.8 MB (157848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6f8ed2c43944590fd32a48b0d2074618a6245b71a2ed18462d5c96e676b6c`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa47e1e197708807cfe4e1f6eae85c6097ceb9ff78de264cd77ff350acb85f`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 9.5 KB (9523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d2059ad7e51f9f633a992795b9d65cee7c9666fc49ff54680de2ce3ea9383`  
		Last Modified: Thu, 20 Aug 2020 03:26:05 GMT  
		Size: 6.9 MB (6918933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:05bf5c4a2fa8306879d1a6a2df12cb425b6ae3523cea0ab1dbd494cdcfcf7af7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.7 MB (252748748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9f068c4d4dae36f005eed0b5bc6797995229b69d3f46fcba867e03479aa2f0a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:22 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 21:59:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Wed, 19 Aug 2020 22:46:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Wed, 19 Aug 2020 22:46:12 GMT
ARG OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 19 Aug 2020 22:46:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 19 Aug 2020 22:46:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 19 Aug 2020 22:46:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 19 Aug 2020 22:46:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 19 Aug 2020 22:46:44 GMT
USER 1001
# Wed, 19 Aug 2020 22:46:44 GMT
EXPOSE 9080 9443
# Wed, 19 Aug 2020 22:46:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 19 Aug 2020 22:46:45 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172b17642c4976ab19fd089c118bc5daf377f3a385fee3563d8af19598f2050`  
		Last Modified: Wed, 19 Aug 2020 22:05:35 GMT  
		Size: 48.4 MB (48386872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b611fd8ca23c160b4762d74a71c9cd634b4be59334c057b753ef115bae4fa3`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f6082ead0ee7fd5c965e9518845d895223681b0c395081b672e61f8609caae`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779a45a76e45c81bb2bd668adcc03deb55d44c66a727d5a5d873453a026b0b50`  
		Last Modified: Wed, 19 Aug 2020 22:49:45 GMT  
		Size: 157.8 MB (157847156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccc2d7faf8eb3abf7b4ce036697fd93cd747f4a743925d3bb2e15ac5f87983b`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadd59fcc56ef3a1cf58e38625ca4ea1cb83c64dfb48bed436b55ad040c19ce8`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 9.5 KB (9495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5f8433ef858963b930e4ebb8360bf2fdb8d5eb829dac045a68b0ca29230d38`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 7.5 MB (7491626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:latest`

```console
$ docker pull open-liberty@sha256:653bc5b94658baf23fad2f69e91477a95ec86c0db9f738763a825107882c413d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:latest` - linux; amd64

```console
$ docker pull open-liberty@sha256:7cbe0cfd4556d2484c1f7054179541681d9b31a76f72086b9fe77869990082ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.2 MB (272154665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02d04f1ae31520d1f366a0ed0fa838952d13c24556a0460f8cd411523e83344d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:00:38 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 02:16:32 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:32 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 02:16:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 02:16:44 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 02:16:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 02:17:07 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 02:17:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 02:17:08 GMT
USER 1001
# Thu, 20 Aug 2020 02:17:08 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 02:17:08 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 02:17:08 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 02:17:21 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Thu, 20 Aug 2020 02:17:55 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a8737f865890826d26efd4c158416bd1188e715c783fd41548e040ef975dbe`  
		Last Modified: Wed, 19 Aug 2020 22:05:50 GMT  
		Size: 48.7 MB (48691306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6597d5c2fcc114d8288a0802f34d16d564cb007ed2d59d38188aa091be14b25d`  
		Last Modified: Thu, 20 Aug 2020 02:20:24 GMT  
		Size: 8.4 KB (8352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888430f050ceadc370b33895dc685299bfd5a255de3160addf3e8887d57ad3c1`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34bb89999af5eea4a3a2270b33aab65b156ded317b60b50da02b17e14762d37`  
		Last Modified: Thu, 20 Aug 2020 02:20:34 GMT  
		Size: 157.8 MB (157847581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea7686ef22dccde6374800a0a8af564aab1d2ce37971d5491effba12f260f83`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd604c0109bce96a7f35816d7a30c902b84f8cafc5121ae095a6e3bb00b07fc4`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 9.4 KB (9400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6cc4e7ae36550db2126f74e99c81b6d5eb44b5f5b38112ff7272b531c91db`  
		Last Modified: Thu, 20 Aug 2020 02:20:25 GMT  
		Size: 8.1 MB (8057281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996a7ba33d6ba87063fb63dd6b87d739a5c0ebae06b7ac2867d34a17af16c0a3`  
		Last Modified: Thu, 20 Aug 2020 02:20:38 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3fd1c9f3fd3f9472a9dddda0b74f0edf7b5ae82f7d7bf7fb104c3e63bd634d`  
		Last Modified: Thu, 20 Aug 2020 02:20:41 GMT  
		Size: 16.9 MB (16926973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:cfc22d235e304fb21276e202255d52b979ce40e105a1ab420fd1f17418abcca4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.6 MB (273578130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7be0bb5cbe3179d1a1d907492325e9237827a8a8f805ab37c1b5788f12975fe8`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:33 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:33:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:33:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:33:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 03:13:43 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 03:13:46 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 03:13:49 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 03:13:52 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 03:13:53 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:14:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 03:14:02 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 03:14:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 03:14:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 03:15:06 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:15:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 03:15:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 03:16:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 03:16:09 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 03:16:12 GMT
USER 1001
# Thu, 20 Aug 2020 03:16:18 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 03:16:23 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 03:16:29 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 03:16:49 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Thu, 20 Aug 2020 03:17:48 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59a1586230e65d6fbe8aebe774b944895c099ea81decb8818ba03aa8180880`  
		Last Modified: Wed, 19 Aug 2020 22:46:13 GMT  
		Size: 49.2 MB (49150099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ec4d988366d9ca7186bc54ce46603179ccf0681f888dc0d42e8cb0c3e7d01d`  
		Last Modified: Thu, 20 Aug 2020 03:26:08 GMT  
		Size: 8.4 KB (8383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1de4b8fd3a1677f86db2f581b69d6b8ec280d723044406d5873ef487e619738`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a445138c34d32647f9b4d494a0fa8d79332a812060b2c8ff31ef187339c1e9e`  
		Last Modified: Thu, 20 Aug 2020 03:26:17 GMT  
		Size: 157.8 MB (157848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6f8ed2c43944590fd32a48b0d2074618a6245b71a2ed18462d5c96e676b6c`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa47e1e197708807cfe4e1f6eae85c6097ceb9ff78de264cd77ff350acb85f`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 9.5 KB (9523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d2059ad7e51f9f633a992795b9d65cee7c9666fc49ff54680de2ce3ea9383`  
		Last Modified: Thu, 20 Aug 2020 03:26:05 GMT  
		Size: 6.9 MB (6918933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99121a436a07f2e84c54768e407a35724fb9a63574e29822e45ddcbde16aeb44`  
		Last Modified: Thu, 20 Aug 2020 03:26:29 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4d071db851d85c4d43f702c7b21e45077482c290f5d9fdb4f0be564a861dda`  
		Last Modified: Thu, 20 Aug 2020 03:26:33 GMT  
		Size: 14.7 MB (14676987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; s390x

```console
$ docker pull open-liberty@sha256:842c5646b1c1e6d9b3a2aabd4883f4bcbf1c92690eb23cb7e874c6bf02bc1df2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.0 MB (269026630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c069ce61a624fb5ddfc3281f89c87b994492debae51d4aed6fa84b1c88d34f77`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:22 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 21:59:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Wed, 19 Aug 2020 22:46:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Wed, 19 Aug 2020 22:46:12 GMT
ARG OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 19 Aug 2020 22:46:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 19 Aug 2020 22:46:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 19 Aug 2020 22:46:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 19 Aug 2020 22:46:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 19 Aug 2020 22:46:44 GMT
USER 1001
# Wed, 19 Aug 2020 22:46:44 GMT
EXPOSE 9080 9443
# Wed, 19 Aug 2020 22:46:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 19 Aug 2020 22:46:45 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Wed, 19 Aug 2020 22:46:53 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Wed, 19 Aug 2020 22:47:16 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172b17642c4976ab19fd089c118bc5daf377f3a385fee3563d8af19598f2050`  
		Last Modified: Wed, 19 Aug 2020 22:05:35 GMT  
		Size: 48.4 MB (48386872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b611fd8ca23c160b4762d74a71c9cd634b4be59334c057b753ef115bae4fa3`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f6082ead0ee7fd5c965e9518845d895223681b0c395081b672e61f8609caae`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779a45a76e45c81bb2bd668adcc03deb55d44c66a727d5a5d873453a026b0b50`  
		Last Modified: Wed, 19 Aug 2020 22:49:45 GMT  
		Size: 157.8 MB (157847156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccc2d7faf8eb3abf7b4ce036697fd93cd747f4a743925d3bb2e15ac5f87983b`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadd59fcc56ef3a1cf58e38625ca4ea1cb83c64dfb48bed436b55ad040c19ce8`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 9.5 KB (9495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5f8433ef858963b930e4ebb8360bf2fdb8d5eb829dac045a68b0ca29230d38`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 7.5 MB (7491626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6810ce5a1c4bc7a1c60c6f4d422dbcf2fe75f9ec78f516ee244c874f98b56836`  
		Last Modified: Wed, 19 Aug 2020 22:49:51 GMT  
		Size: 965.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e59c06f29d6550fa79ae98c6540ed99bf540e00af155ff14140df006a62e3f`  
		Last Modified: Wed, 19 Aug 2020 22:49:53 GMT  
		Size: 16.3 MB (16276917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
