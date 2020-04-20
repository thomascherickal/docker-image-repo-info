<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `open-liberty`

-	[`open-liberty:19.0.0.12-full-java8-openj9`](#open-liberty190012-full-java8-openj9)
-	[`open-liberty:19.0.0.12-kernel-java8-openj9`](#open-liberty190012-kernel-java8-openj9)
-	[`open-liberty:20.0.0.3-full-java8-openj9`](#open-liberty20003-full-java8-openj9)
-	[`open-liberty:20.0.0.3-kernel-java8-openj9`](#open-liberty20003-kernel-java8-openj9)
-	[`open-liberty:full`](#open-libertyfull)
-	[`open-liberty:full-java8-openj9`](#open-libertyfull-java8-openj9)
-	[`open-liberty:kernel`](#open-libertykernel)
-	[`open-liberty:kernel-java8-openj9`](#open-libertykernel-java8-openj9)
-	[`open-liberty:latest`](#open-libertylatest)

## `open-liberty:19.0.0.12-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:608b6a0bdfe9bc80da75eca07459b3fe9493f6534d9490d39d28152703c0dba3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:19.0.0.12-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:704f92221c076c5db4776808671fbecfbc8c4db8552670f9bfc6785e3336661f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.3 MB (238315877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9e3df6467d652dc0d5c5965e7ccd1f5201c50e0ebd0f6b77ae2556218b60ed`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:37:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:22:51 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 20 Apr 2020 17:23:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 20 Apr 2020 19:03:06 GMT
ARG LIBERTY_VERSION=19.0.0.12
# Mon, 20 Apr 2020 19:03:07 GMT
ARG LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e
# Mon, 20 Apr 2020 19:03:07 GMT
ARG LIBERTY_BUILD_LABEL=cl191220191120-0300
# Mon, 20 Apr 2020 19:03:07 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip
# Mon, 20 Apr 2020 19:03:08 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl191220191120-0300
# Mon, 20 Apr 2020 19:03:08 GMT
COPY dir:0a95802328e5a4e645b6642a95ef493aa335028988fa24f2a183a54e5e237536 in /opt/ol/helpers 
# Mon, 20 Apr 2020 19:03:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Mon, 20 Apr 2020 19:03:29 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true
# Mon, 20 Apr 2020 19:03:32 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 20 Apr 2020 19:03:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Mon, 20 Apr 2020 19:03:34 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Mon, 20 Apr 2020 19:03:34 GMT
USER 1001
# Mon, 20 Apr 2020 19:03:35 GMT
EXPOSE 9080 9443
# Mon, 20 Apr 2020 19:03:35 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Mon, 20 Apr 2020 19:03:35 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Mon, 20 Apr 2020 19:03:42 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7abfeb06800729d4f24d971e8017c537c4fa86368ae0bca66a7b36ca2b4189`  
		Last Modified: Fri, 20 Mar 2020 19:40:17 GMT  
		Size: 13.3 MB (13325178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ddacaa0d9e81143e1cdfaf134d500ebdc3ea02dd32c6294a4c0666ef29c52`  
		Last Modified: Mon, 20 Apr 2020 17:26:40 GMT  
		Size: 48.5 MB (48502646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ea1c9f0f988ca929295e87250e944745e15b684b3414c713873ff9181e58e4`  
		Last Modified: Mon, 20 Apr 2020 19:04:40 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888da86c024fd09072810cc64f79527698ee5ac250fbe24fbe10502067c2bfa4`  
		Last Modified: Mon, 20 Apr 2020 19:04:51 GMT  
		Size: 149.8 MB (149753290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3d793b2aedba4d00f2638221ab145474c6101154dbf49b5555851ac9a5fa4f`  
		Last Modified: Mon, 20 Apr 2020 19:04:40 GMT  
		Size: 936.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7457b6ffd9aee215d6d750f12c02abfdb5cd4cf039709c80bda875ed669a43`  
		Last Modified: Mon, 20 Apr 2020 19:04:40 GMT  
		Size: 3.4 KB (3400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe261a8d004d6dd1062c6260f7d31b4b080c4cc4b9a7776b2aacf335c35ffd2`  
		Last Modified: Mon, 20 Apr 2020 19:05:13 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:19.0.0.12-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:4a14f80c053de7c4b51b97b495c510ca031f90fe25470ec63ec0c72cfac96dc9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.6 MB (242590014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cfd11fb04ed1e1d8185228f623b4e818b95717995a43d63bad16324d269c54`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:22:18 GMT
ADD file:226ecdf321a0fde3bea0d6e88db018b3d077f676a1f1e06942217ebb26a02301 in / 
# Fri, 20 Mar 2020 19:22:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:22:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:22:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:22:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:41:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:44:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:47:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:48:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:48:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:48:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 20 Mar 2020 22:09:18 GMT
ARG LIBERTY_VERSION=19.0.0.12
# Fri, 20 Mar 2020 22:09:21 GMT
ARG LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e
# Fri, 20 Mar 2020 22:09:27 GMT
ARG LIBERTY_BUILD_LABEL=cl191220191120-0300
# Fri, 20 Mar 2020 22:09:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip
# Fri, 20 Mar 2020 22:09:34 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl191220191120-0300
# Fri, 20 Mar 2020 22:09:35 GMT
COPY dir:0a95802328e5a4e645b6642a95ef493aa335028988fa24f2a183a54e5e237536 in /opt/ol/helpers 
# Fri, 20 Mar 2020 22:10:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 20 Mar 2020 22:10:17 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true
# Fri, 20 Mar 2020 22:10:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 20 Mar 2020 22:10:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 20 Mar 2020 22:10:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 20 Mar 2020 22:10:45 GMT
USER 1001
# Fri, 20 Mar 2020 22:10:48 GMT
EXPOSE 9080 9443
# Fri, 20 Mar 2020 22:10:53 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 20 Mar 2020 22:10:55 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 20 Mar 2020 22:11:18 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:044eae4257f9584af1a24a5cdb9754c96aea36080e68260ddbabab04827bac00`  
		Last Modified: Mon, 16 Mar 2020 15:38:59 GMT  
		Size: 30.4 MB (30399915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf63a142f3acf0fc36d344bc173f2e1990e692aff0c1237ed6dc96cf38cfb2e`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64d9f5f16809d964026266c73b1c06d3cc0dc517437a91d8639758b80958679`  
		Last Modified: Fri, 20 Mar 2020 19:25:01 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c34444f41441c2f598f5dda94ec1b47ee527ce6e5025d70e5eea41a400d16b1`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa3d39187779cfab3b684c0f6e3d861528565e584fbb8dc2e72d633644f21c`  
		Last Modified: Fri, 20 Mar 2020 19:52:26 GMT  
		Size: 14.0 MB (13970663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1612cc71117278a0165cc5c3d4ec4b8a4ae0ad0ddb6ec8ad048b3847a9bcd6a`  
		Last Modified: Fri, 20 Mar 2020 19:55:35 GMT  
		Size: 48.4 MB (48421548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d4af4c68b2d92cceffe580f16b975a726b3088c438a7506e81c77208ae0b54`  
		Last Modified: Fri, 20 Mar 2020 22:12:17 GMT  
		Size: 2.5 KB (2514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157c6ec03182de9f681c630baa5b37c931e019dc366cd2ec44b6776a96957557`  
		Last Modified: Fri, 20 Mar 2020 22:12:30 GMT  
		Size: 149.8 MB (149753674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab52fa9e9ded434be517810c49c34d3d0adf5d03e0cc3dade187de8299492ab`  
		Last Modified: Fri, 20 Mar 2020 22:12:17 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48c41fd77eb9e58733ad4f430e1df1cd5646739afbc934597b9f5fa5cdc68b8`  
		Last Modified: Fri, 20 Mar 2020 22:12:17 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442394dc7a5966f3cefbb916ccc8e3bccd745eba57ff95bef4ec77fa800fe41a`  
		Last Modified: Fri, 20 Mar 2020 22:12:39 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:19.0.0.12-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:8b681a42e44df854d5f454a1d7bcf9ddcf20adbcc0586b8f50b874176f489879
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.4 MB (236375793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f85d12dc358441c438f9604c19ed0deb776babe30f262e70975204ff48b08c93`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:38:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:38:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:40:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:40:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 20 Mar 2020 21:09:50 GMT
ARG LIBERTY_VERSION=19.0.0.12
# Fri, 20 Mar 2020 21:09:51 GMT
ARG LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e
# Fri, 20 Mar 2020 21:09:51 GMT
ARG LIBERTY_BUILD_LABEL=cl191220191120-0300
# Fri, 20 Mar 2020 21:09:51 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip
# Fri, 20 Mar 2020 21:09:51 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl191220191120-0300
# Fri, 20 Mar 2020 21:09:51 GMT
COPY dir:0a95802328e5a4e645b6642a95ef493aa335028988fa24f2a183a54e5e237536 in /opt/ol/helpers 
# Fri, 20 Mar 2020 21:10:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 20 Mar 2020 21:10:05 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true
# Fri, 20 Mar 2020 21:10:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 20 Mar 2020 21:10:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 20 Mar 2020 21:10:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 20 Mar 2020 21:10:07 GMT
USER 1001
# Fri, 20 Mar 2020 21:10:07 GMT
EXPOSE 9080 9443
# Fri, 20 Mar 2020 21:10:07 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 20 Mar 2020 21:10:07 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 20 Mar 2020 21:10:13 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c87faf3e6b36db60f122e065a6d270147409d2b806f06443b02248d6187ad`  
		Last Modified: Fri, 20 Mar 2020 19:42:19 GMT  
		Size: 13.0 MB (13043890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1095d74aa4b9db1c93872abb7a2b7b6afc292f944a2827d13f6216bf00d1406a`  
		Last Modified: Fri, 20 Mar 2020 19:44:13 GMT  
		Size: 48.2 MB (48169610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38a733c47c011528b2a390e5c67b098d59ad4bd6baec6cab2bf5750d8ae8f7f`  
		Last Modified: Fri, 20 Mar 2020 21:10:54 GMT  
		Size: 2.5 KB (2513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e194da5390cc139b795ca38d4c6fed4f2600fd4231b587ab897d9612136628f9`  
		Last Modified: Fri, 20 Mar 2020 21:11:06 GMT  
		Size: 149.8 MB (149752520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaa79ee38d149c0536aa6623353fb68275ec63d60b2aa7e5f7d0f1e41e9642b`  
		Last Modified: Fri, 20 Mar 2020 21:11:09 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1879f87bee5f2bb0a6654e6917d5adc2ea3abd8959298231c8e7c53f12472b6a`  
		Last Modified: Fri, 20 Mar 2020 21:10:54 GMT  
		Size: 3.5 KB (3472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c582517e07622b6d38fd0274b5417e4bfcfba0068fe11960f1e1a91c4744f5`  
		Last Modified: Fri, 20 Mar 2020 21:11:13 GMT  
		Size: 963.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:19.0.0.12-kernel-java8-openj9`

```console
$ docker pull open-liberty@sha256:ca322f44aa809a02d1067c07d7b3243228da5945d82487c4c62d5363afeb3fa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:19.0.0.12-kernel-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:b4a7eec726f3e4ffb48322f3873a06271db81271ce7b799d112e62737367188f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.3 MB (238314910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:464a5dc47535e2811510746cbd26cee5969c11ef39e5e26238f576b60434d223`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:37:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:22:51 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 20 Apr 2020 17:23:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 20 Apr 2020 19:03:06 GMT
ARG LIBERTY_VERSION=19.0.0.12
# Mon, 20 Apr 2020 19:03:07 GMT
ARG LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e
# Mon, 20 Apr 2020 19:03:07 GMT
ARG LIBERTY_BUILD_LABEL=cl191220191120-0300
# Mon, 20 Apr 2020 19:03:07 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip
# Mon, 20 Apr 2020 19:03:08 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl191220191120-0300
# Mon, 20 Apr 2020 19:03:08 GMT
COPY dir:0a95802328e5a4e645b6642a95ef493aa335028988fa24f2a183a54e5e237536 in /opt/ol/helpers 
# Mon, 20 Apr 2020 19:03:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Mon, 20 Apr 2020 19:03:29 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true
# Mon, 20 Apr 2020 19:03:32 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 20 Apr 2020 19:03:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Mon, 20 Apr 2020 19:03:34 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Mon, 20 Apr 2020 19:03:34 GMT
USER 1001
# Mon, 20 Apr 2020 19:03:35 GMT
EXPOSE 9080 9443
# Mon, 20 Apr 2020 19:03:35 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Mon, 20 Apr 2020 19:03:35 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7abfeb06800729d4f24d971e8017c537c4fa86368ae0bca66a7b36ca2b4189`  
		Last Modified: Fri, 20 Mar 2020 19:40:17 GMT  
		Size: 13.3 MB (13325178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ddacaa0d9e81143e1cdfaf134d500ebdc3ea02dd32c6294a4c0666ef29c52`  
		Last Modified: Mon, 20 Apr 2020 17:26:40 GMT  
		Size: 48.5 MB (48502646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ea1c9f0f988ca929295e87250e944745e15b684b3414c713873ff9181e58e4`  
		Last Modified: Mon, 20 Apr 2020 19:04:40 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888da86c024fd09072810cc64f79527698ee5ac250fbe24fbe10502067c2bfa4`  
		Last Modified: Mon, 20 Apr 2020 19:04:51 GMT  
		Size: 149.8 MB (149753290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3d793b2aedba4d00f2638221ab145474c6101154dbf49b5555851ac9a5fa4f`  
		Last Modified: Mon, 20 Apr 2020 19:04:40 GMT  
		Size: 936.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7457b6ffd9aee215d6d750f12c02abfdb5cd4cf039709c80bda875ed669a43`  
		Last Modified: Mon, 20 Apr 2020 19:04:40 GMT  
		Size: 3.4 KB (3400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:19.0.0.12-kernel-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:f0fadfe44a3f0343c7154c54d60789c9a1fa25bfaee97046e2325211e99184d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.6 MB (242589047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d0ed6ed4653b24e112693ca1c4fbf51141209252eb3a977cdb9822792708434`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:22:18 GMT
ADD file:226ecdf321a0fde3bea0d6e88db018b3d077f676a1f1e06942217ebb26a02301 in / 
# Fri, 20 Mar 2020 19:22:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:22:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:22:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:22:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:41:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:44:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:47:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:48:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:48:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:48:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 20 Mar 2020 22:09:18 GMT
ARG LIBERTY_VERSION=19.0.0.12
# Fri, 20 Mar 2020 22:09:21 GMT
ARG LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e
# Fri, 20 Mar 2020 22:09:27 GMT
ARG LIBERTY_BUILD_LABEL=cl191220191120-0300
# Fri, 20 Mar 2020 22:09:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip
# Fri, 20 Mar 2020 22:09:34 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl191220191120-0300
# Fri, 20 Mar 2020 22:09:35 GMT
COPY dir:0a95802328e5a4e645b6642a95ef493aa335028988fa24f2a183a54e5e237536 in /opt/ol/helpers 
# Fri, 20 Mar 2020 22:10:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 20 Mar 2020 22:10:17 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true
# Fri, 20 Mar 2020 22:10:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 20 Mar 2020 22:10:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 20 Mar 2020 22:10:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 20 Mar 2020 22:10:45 GMT
USER 1001
# Fri, 20 Mar 2020 22:10:48 GMT
EXPOSE 9080 9443
# Fri, 20 Mar 2020 22:10:53 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 20 Mar 2020 22:10:55 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:044eae4257f9584af1a24a5cdb9754c96aea36080e68260ddbabab04827bac00`  
		Last Modified: Mon, 16 Mar 2020 15:38:59 GMT  
		Size: 30.4 MB (30399915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf63a142f3acf0fc36d344bc173f2e1990e692aff0c1237ed6dc96cf38cfb2e`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64d9f5f16809d964026266c73b1c06d3cc0dc517437a91d8639758b80958679`  
		Last Modified: Fri, 20 Mar 2020 19:25:01 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c34444f41441c2f598f5dda94ec1b47ee527ce6e5025d70e5eea41a400d16b1`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa3d39187779cfab3b684c0f6e3d861528565e584fbb8dc2e72d633644f21c`  
		Last Modified: Fri, 20 Mar 2020 19:52:26 GMT  
		Size: 14.0 MB (13970663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1612cc71117278a0165cc5c3d4ec4b8a4ae0ad0ddb6ec8ad048b3847a9bcd6a`  
		Last Modified: Fri, 20 Mar 2020 19:55:35 GMT  
		Size: 48.4 MB (48421548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d4af4c68b2d92cceffe580f16b975a726b3088c438a7506e81c77208ae0b54`  
		Last Modified: Fri, 20 Mar 2020 22:12:17 GMT  
		Size: 2.5 KB (2514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157c6ec03182de9f681c630baa5b37c931e019dc366cd2ec44b6776a96957557`  
		Last Modified: Fri, 20 Mar 2020 22:12:30 GMT  
		Size: 149.8 MB (149753674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab52fa9e9ded434be517810c49c34d3d0adf5d03e0cc3dade187de8299492ab`  
		Last Modified: Fri, 20 Mar 2020 22:12:17 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48c41fd77eb9e58733ad4f430e1df1cd5646739afbc934597b9f5fa5cdc68b8`  
		Last Modified: Fri, 20 Mar 2020 22:12:17 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:19.0.0.12-kernel-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:01a2c567327343870ddc94827fe31d908a856d934c20f091fd5ba933eab41a13
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.4 MB (236374830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:121c021602590c749691389cf2118bdabc7d2a8376ec936072b827f7c9ae62ee`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:38:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:38:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:40:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:40:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 20 Mar 2020 21:09:50 GMT
ARG LIBERTY_VERSION=19.0.0.12
# Fri, 20 Mar 2020 21:09:51 GMT
ARG LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e
# Fri, 20 Mar 2020 21:09:51 GMT
ARG LIBERTY_BUILD_LABEL=cl191220191120-0300
# Fri, 20 Mar 2020 21:09:51 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip
# Fri, 20 Mar 2020 21:09:51 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl191220191120-0300
# Fri, 20 Mar 2020 21:09:51 GMT
COPY dir:0a95802328e5a4e645b6642a95ef493aa335028988fa24f2a183a54e5e237536 in /opt/ol/helpers 
# Fri, 20 Mar 2020 21:10:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 20 Mar 2020 21:10:05 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true
# Fri, 20 Mar 2020 21:10:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 20 Mar 2020 21:10:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl191220191120-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/19.0.0.12/openliberty-runtime-19.0.0.12.zip LIBERTY_SHA=b3a613cbad764a10ae57719ff9818c3bcfefdf8e LIBERTY_VERSION=19.0.0.12
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 20 Mar 2020 21:10:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 20 Mar 2020 21:10:07 GMT
USER 1001
# Fri, 20 Mar 2020 21:10:07 GMT
EXPOSE 9080 9443
# Fri, 20 Mar 2020 21:10:07 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 20 Mar 2020 21:10:07 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c87faf3e6b36db60f122e065a6d270147409d2b806f06443b02248d6187ad`  
		Last Modified: Fri, 20 Mar 2020 19:42:19 GMT  
		Size: 13.0 MB (13043890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1095d74aa4b9db1c93872abb7a2b7b6afc292f944a2827d13f6216bf00d1406a`  
		Last Modified: Fri, 20 Mar 2020 19:44:13 GMT  
		Size: 48.2 MB (48169610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38a733c47c011528b2a390e5c67b098d59ad4bd6baec6cab2bf5750d8ae8f7f`  
		Last Modified: Fri, 20 Mar 2020 21:10:54 GMT  
		Size: 2.5 KB (2513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e194da5390cc139b795ca38d4c6fed4f2600fd4231b587ab897d9612136628f9`  
		Last Modified: Fri, 20 Mar 2020 21:11:06 GMT  
		Size: 149.8 MB (149752520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaa79ee38d149c0536aa6623353fb68275ec63d60b2aa7e5f7d0f1e41e9642b`  
		Last Modified: Fri, 20 Mar 2020 21:11:09 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1879f87bee5f2bb0a6654e6917d5adc2ea3abd8959298231c8e7c53f12472b6a`  
		Last Modified: Fri, 20 Mar 2020 21:10:54 GMT  
		Size: 3.5 KB (3472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.3-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:ad02fc58bd93500696dc1cf640c383214f6befa124f07ec285dd0c2bc3a27895
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.3-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:b3c8e2c342ae4996ca4b6b12d50f9fc8ccc3c0ef7f51ae000ae83475860b2588
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.1 MB (251131918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5672f7f42f69479d0879cbd218ca5410f931e9983d8435e09fa44a6f27054bc0`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:37:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:22:51 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 20 Apr 2020 17:23:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 20 Apr 2020 19:02:14 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Mon, 20 Apr 2020 19:02:14 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Mon, 20 Apr 2020 19:02:14 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Mon, 20 Apr 2020 19:02:15 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Mon, 20 Apr 2020 19:02:15 GMT
ARG OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:02:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433
# Mon, 20 Apr 2020 19:02:15 GMT
COPY dir:0e3761f4861bb1595d4d3b9ca71d59f44542edaab3d44a678bec40e43392bcf5 in /opt/ol/helpers 
# Mon, 20 Apr 2020 19:02:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Mon, 20 Apr 2020 19:02:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:02:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 20 Apr 2020 19:02:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Mon, 20 Apr 2020 19:02:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Mon, 20 Apr 2020 19:02:52 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Mon, 20 Apr 2020 19:02:52 GMT
USER 1001
# Mon, 20 Apr 2020 19:02:52 GMT
EXPOSE 9080 9443
# Mon, 20 Apr 2020 19:02:52 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Mon, 20 Apr 2020 19:02:52 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Mon, 20 Apr 2020 19:03:02 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7abfeb06800729d4f24d971e8017c537c4fa86368ae0bca66a7b36ca2b4189`  
		Last Modified: Fri, 20 Mar 2020 19:40:17 GMT  
		Size: 13.3 MB (13325178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ddacaa0d9e81143e1cdfaf134d500ebdc3ea02dd32c6294a4c0666ef29c52`  
		Last Modified: Mon, 20 Apr 2020 17:26:40 GMT  
		Size: 48.5 MB (48502646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989475d9f0f735ca6eefe3838c2b22b258df049c0df551a3dff63e2b41baf97`  
		Last Modified: Mon, 20 Apr 2020 19:04:23 GMT  
		Size: 6.3 KB (6318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d288a7c474f7e415febe6b7bbed474d217f72f5d1929f801e00eadc11dfc716`  
		Last Modified: Mon, 20 Apr 2020 19:04:34 GMT  
		Size: 155.0 MB (155026893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e2cd45685893c3af88b57c4992fcc9be4638c72ea586ac7011b5fdf3813811`  
		Last Modified: Mon, 20 Apr 2020 19:04:23 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047b887e1fb765567b7000a0c11c6c14a6ca05286156ab08d8cdb645bb0f828d`  
		Last Modified: Mon, 20 Apr 2020 19:04:23 GMT  
		Size: 7.2 KB (7237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d52a37a51b703098b6420324767f38758698d3b8aceda27fec15d98617230d`  
		Last Modified: Mon, 20 Apr 2020 19:04:25 GMT  
		Size: 7.5 MB (7534772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34025f69c7816f194000b5a45a72795b07796ebd81a5eed1672265443ef276bd`  
		Last Modified: Mon, 20 Apr 2020 19:04:38 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.3-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:f6fc49ed30e91c265d398dbfbfbf00d053e258632bfe28ec33adc00033756517
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.1 MB (254066233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8b9056d9c9dc023e489e0e070cd9160b0d780fa00dfe10ffe5a6d627af843f5`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:22:18 GMT
ADD file:226ecdf321a0fde3bea0d6e88db018b3d077f676a1f1e06942217ebb26a02301 in / 
# Fri, 20 Mar 2020 19:22:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:22:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:22:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:22:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:41:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:44:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:47:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:48:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:48:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:48:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 20 Mar 2020 22:06:54 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Fri, 20 Mar 2020 22:06:57 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Fri, 20 Mar 2020 22:07:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Fri, 20 Mar 2020 22:07:02 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Fri, 20 Mar 2020 22:07:05 GMT
ARG OPENJ9_SCC=true
# Fri, 20 Mar 2020 22:07:06 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433
# Tue, 14 Apr 2020 21:19:31 GMT
COPY dir:0e3761f4861bb1595d4d3b9ca71d59f44542edaab3d44a678bec40e43392bcf5 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:21:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:21:45 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:21:54 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:22:10 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:22:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:22:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:22:49 GMT
USER 1001
# Tue, 14 Apr 2020 21:22:54 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:22:56 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:22:59 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Tue, 14 Apr 2020 21:23:14 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:044eae4257f9584af1a24a5cdb9754c96aea36080e68260ddbabab04827bac00`  
		Last Modified: Mon, 16 Mar 2020 15:38:59 GMT  
		Size: 30.4 MB (30399915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf63a142f3acf0fc36d344bc173f2e1990e692aff0c1237ed6dc96cf38cfb2e`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64d9f5f16809d964026266c73b1c06d3cc0dc517437a91d8639758b80958679`  
		Last Modified: Fri, 20 Mar 2020 19:25:01 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c34444f41441c2f598f5dda94ec1b47ee527ce6e5025d70e5eea41a400d16b1`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa3d39187779cfab3b684c0f6e3d861528565e584fbb8dc2e72d633644f21c`  
		Last Modified: Fri, 20 Mar 2020 19:52:26 GMT  
		Size: 14.0 MB (13970663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1612cc71117278a0165cc5c3d4ec4b8a4ae0ad0ddb6ec8ad048b3847a9bcd6a`  
		Last Modified: Fri, 20 Mar 2020 19:55:35 GMT  
		Size: 48.4 MB (48421548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6e9b13dceb0149c6e35b36274c457b92be0dc1406b9630619acdcb8b3ce0f9`  
		Last Modified: Tue, 14 Apr 2020 21:24:11 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed75a5a5d53f0291a0bab5ec39af8938201aa04cbd6b3c8ec7536c87058a2b7f`  
		Last Modified: Tue, 14 Apr 2020 21:24:25 GMT  
		Size: 155.0 MB (155027527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baecb34648698db288b7bb38ff83647e8e865cfb1cb4c1223ea784570a32df0`  
		Last Modified: Tue, 14 Apr 2020 21:24:11 GMT  
		Size: 1.0 KB (1002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8919939cbf424f846aaa06a33864b8aed18e8a6a4694d8feb40cf4d250619ff0`  
		Last Modified: Tue, 14 Apr 2020 21:24:11 GMT  
		Size: 7.3 KB (7342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e11b1fdc7f3536d0ffbfbec4d0891ecd711aae8566b2e5d134127fed1796749`  
		Last Modified: Tue, 14 Apr 2020 21:24:13 GMT  
		Size: 6.2 MB (6194680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe7859ebed42df2431cee73dbf5fb62dd3b325086a69cf3434fff3041cf8541`  
		Last Modified: Tue, 14 Apr 2020 21:24:36 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.3-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:4fcabb3fc21047a9eb0aaf245f0d5a18c9217b61f864d7282aa0d18f60017807
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248769787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a18f7be6917cb8d20883537fb4e692f672f74ff5d2c7dcd31950353ae756ed77`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:38:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:38:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:40:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:40:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 20 Mar 2020 21:09:03 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Fri, 20 Mar 2020 21:09:04 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Fri, 20 Mar 2020 21:09:04 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Fri, 20 Mar 2020 21:09:04 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Fri, 20 Mar 2020 21:09:04 GMT
ARG OPENJ9_SCC=true
# Fri, 20 Mar 2020 21:09:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433
# Tue, 14 Apr 2020 21:28:57 GMT
COPY dir:0e3761f4861bb1595d4d3b9ca71d59f44542edaab3d44a678bec40e43392bcf5 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:29:08 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:29:11 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:29:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:29:12 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:29:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:29:24 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:29:24 GMT
USER 1001
# Tue, 14 Apr 2020 21:29:24 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:29:25 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:29:25 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Tue, 14 Apr 2020 21:29:32 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c87faf3e6b36db60f122e065a6d270147409d2b806f06443b02248d6187ad`  
		Last Modified: Fri, 20 Mar 2020 19:42:19 GMT  
		Size: 13.0 MB (13043890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1095d74aa4b9db1c93872abb7a2b7b6afc292f944a2827d13f6216bf00d1406a`  
		Last Modified: Fri, 20 Mar 2020 19:44:13 GMT  
		Size: 48.2 MB (48169610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2a9ccb2791799db21d6b18ee6aefe140524c1505e421a223ce911e3c39287b`  
		Last Modified: Tue, 14 Apr 2020 21:30:12 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126039dd8987d44542577c38e1fb5c440313f91d0bb6f3e053f072f85d4e42ef`  
		Last Modified: Tue, 14 Apr 2020 21:30:37 GMT  
		Size: 155.0 MB (155026327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92057d97756621afa2f4a2e007a84a31a4ebd029386df3f36862e79831db6e07`  
		Last Modified: Tue, 14 Apr 2020 21:30:12 GMT  
		Size: 996.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3381a8a42899a552e62b60b01a7abbfd6f3eb28a0d55e7c09e3b2d940a3cea74`  
		Last Modified: Tue, 14 Apr 2020 21:30:28 GMT  
		Size: 7.3 KB (7319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e621462fe4eadd3d9466815b3f3a6287f6f2173bbbcf3f6211cfc38a962a633`  
		Last Modified: Tue, 14 Apr 2020 21:30:28 GMT  
		Size: 7.1 MB (7112513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc04a3da68bb7ad02b4ccd0a2a051d5d3dd10be5bb15c2baffdba61c59ce3b`  
		Last Modified: Tue, 14 Apr 2020 21:30:42 GMT  
		Size: 963.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.3-kernel-java8-openj9`

```console
$ docker pull open-liberty@sha256:a8ab7c775e289922e1b3605a630c0abc5a937f8713bd90dbdf20632ea97b0d5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.3-kernel-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:ae0abf789084a22fef5069823cdbe1ec4308d9cc9a794fee7cb5072767938c40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.1 MB (251130952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84403585f92b4cd8714af5bb9526a310aaa8752b95e40ab035e0efcdd102b5af`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:37:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:22:51 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 20 Apr 2020 17:23:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 20 Apr 2020 19:02:14 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Mon, 20 Apr 2020 19:02:14 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Mon, 20 Apr 2020 19:02:14 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Mon, 20 Apr 2020 19:02:15 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Mon, 20 Apr 2020 19:02:15 GMT
ARG OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:02:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433
# Mon, 20 Apr 2020 19:02:15 GMT
COPY dir:0e3761f4861bb1595d4d3b9ca71d59f44542edaab3d44a678bec40e43392bcf5 in /opt/ol/helpers 
# Mon, 20 Apr 2020 19:02:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Mon, 20 Apr 2020 19:02:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:02:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 20 Apr 2020 19:02:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Mon, 20 Apr 2020 19:02:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Mon, 20 Apr 2020 19:02:52 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Mon, 20 Apr 2020 19:02:52 GMT
USER 1001
# Mon, 20 Apr 2020 19:02:52 GMT
EXPOSE 9080 9443
# Mon, 20 Apr 2020 19:02:52 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Mon, 20 Apr 2020 19:02:52 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7abfeb06800729d4f24d971e8017c537c4fa86368ae0bca66a7b36ca2b4189`  
		Last Modified: Fri, 20 Mar 2020 19:40:17 GMT  
		Size: 13.3 MB (13325178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ddacaa0d9e81143e1cdfaf134d500ebdc3ea02dd32c6294a4c0666ef29c52`  
		Last Modified: Mon, 20 Apr 2020 17:26:40 GMT  
		Size: 48.5 MB (48502646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989475d9f0f735ca6eefe3838c2b22b258df049c0df551a3dff63e2b41baf97`  
		Last Modified: Mon, 20 Apr 2020 19:04:23 GMT  
		Size: 6.3 KB (6318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d288a7c474f7e415febe6b7bbed474d217f72f5d1929f801e00eadc11dfc716`  
		Last Modified: Mon, 20 Apr 2020 19:04:34 GMT  
		Size: 155.0 MB (155026893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e2cd45685893c3af88b57c4992fcc9be4638c72ea586ac7011b5fdf3813811`  
		Last Modified: Mon, 20 Apr 2020 19:04:23 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047b887e1fb765567b7000a0c11c6c14a6ca05286156ab08d8cdb645bb0f828d`  
		Last Modified: Mon, 20 Apr 2020 19:04:23 GMT  
		Size: 7.2 KB (7237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d52a37a51b703098b6420324767f38758698d3b8aceda27fec15d98617230d`  
		Last Modified: Mon, 20 Apr 2020 19:04:25 GMT  
		Size: 7.5 MB (7534772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.3-kernel-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:6b32aef21ee513354962c6b8a00b2ccf5c87b27b324defa11e8598371a57a40f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.1 MB (254065266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab7c409c1b80c5c4031395ab0459234dc60793dd3f1f8ec21dc84a852b1c7a98`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:22:18 GMT
ADD file:226ecdf321a0fde3bea0d6e88db018b3d077f676a1f1e06942217ebb26a02301 in / 
# Fri, 20 Mar 2020 19:22:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:22:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:22:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:22:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:41:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:44:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:47:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:48:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:48:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:48:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 20 Mar 2020 22:06:54 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Fri, 20 Mar 2020 22:06:57 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Fri, 20 Mar 2020 22:07:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Fri, 20 Mar 2020 22:07:02 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Fri, 20 Mar 2020 22:07:05 GMT
ARG OPENJ9_SCC=true
# Fri, 20 Mar 2020 22:07:06 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433
# Tue, 14 Apr 2020 21:19:31 GMT
COPY dir:0e3761f4861bb1595d4d3b9ca71d59f44542edaab3d44a678bec40e43392bcf5 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:21:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:21:45 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:21:54 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:22:10 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:22:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:22:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:22:49 GMT
USER 1001
# Tue, 14 Apr 2020 21:22:54 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:22:56 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:22:59 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:044eae4257f9584af1a24a5cdb9754c96aea36080e68260ddbabab04827bac00`  
		Last Modified: Mon, 16 Mar 2020 15:38:59 GMT  
		Size: 30.4 MB (30399915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf63a142f3acf0fc36d344bc173f2e1990e692aff0c1237ed6dc96cf38cfb2e`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64d9f5f16809d964026266c73b1c06d3cc0dc517437a91d8639758b80958679`  
		Last Modified: Fri, 20 Mar 2020 19:25:01 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c34444f41441c2f598f5dda94ec1b47ee527ce6e5025d70e5eea41a400d16b1`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa3d39187779cfab3b684c0f6e3d861528565e584fbb8dc2e72d633644f21c`  
		Last Modified: Fri, 20 Mar 2020 19:52:26 GMT  
		Size: 14.0 MB (13970663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1612cc71117278a0165cc5c3d4ec4b8a4ae0ad0ddb6ec8ad048b3847a9bcd6a`  
		Last Modified: Fri, 20 Mar 2020 19:55:35 GMT  
		Size: 48.4 MB (48421548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6e9b13dceb0149c6e35b36274c457b92be0dc1406b9630619acdcb8b3ce0f9`  
		Last Modified: Tue, 14 Apr 2020 21:24:11 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed75a5a5d53f0291a0bab5ec39af8938201aa04cbd6b3c8ec7536c87058a2b7f`  
		Last Modified: Tue, 14 Apr 2020 21:24:25 GMT  
		Size: 155.0 MB (155027527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baecb34648698db288b7bb38ff83647e8e865cfb1cb4c1223ea784570a32df0`  
		Last Modified: Tue, 14 Apr 2020 21:24:11 GMT  
		Size: 1.0 KB (1002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8919939cbf424f846aaa06a33864b8aed18e8a6a4694d8feb40cf4d250619ff0`  
		Last Modified: Tue, 14 Apr 2020 21:24:11 GMT  
		Size: 7.3 KB (7342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e11b1fdc7f3536d0ffbfbec4d0891ecd711aae8566b2e5d134127fed1796749`  
		Last Modified: Tue, 14 Apr 2020 21:24:13 GMT  
		Size: 6.2 MB (6194680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.3-kernel-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:a19ddfb92edd33342741e07c95a12eedf3a453615bf61190e2ec189577c79942
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248768824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4f47a445dbcd66874246ef9a89310a67b44025828e370fe93285fd58963772`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:38:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:38:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:40:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:40:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 20 Mar 2020 21:09:03 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Fri, 20 Mar 2020 21:09:04 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Fri, 20 Mar 2020 21:09:04 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Fri, 20 Mar 2020 21:09:04 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Fri, 20 Mar 2020 21:09:04 GMT
ARG OPENJ9_SCC=true
# Fri, 20 Mar 2020 21:09:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433
# Tue, 14 Apr 2020 21:28:57 GMT
COPY dir:0e3761f4861bb1595d4d3b9ca71d59f44542edaab3d44a678bec40e43392bcf5 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:29:08 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:29:11 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:29:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:29:12 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:29:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:29:24 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:29:24 GMT
USER 1001
# Tue, 14 Apr 2020 21:29:24 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:29:25 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:29:25 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c87faf3e6b36db60f122e065a6d270147409d2b806f06443b02248d6187ad`  
		Last Modified: Fri, 20 Mar 2020 19:42:19 GMT  
		Size: 13.0 MB (13043890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1095d74aa4b9db1c93872abb7a2b7b6afc292f944a2827d13f6216bf00d1406a`  
		Last Modified: Fri, 20 Mar 2020 19:44:13 GMT  
		Size: 48.2 MB (48169610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2a9ccb2791799db21d6b18ee6aefe140524c1505e421a223ce911e3c39287b`  
		Last Modified: Tue, 14 Apr 2020 21:30:12 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126039dd8987d44542577c38e1fb5c440313f91d0bb6f3e053f072f85d4e42ef`  
		Last Modified: Tue, 14 Apr 2020 21:30:37 GMT  
		Size: 155.0 MB (155026327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92057d97756621afa2f4a2e007a84a31a4ebd029386df3f36862e79831db6e07`  
		Last Modified: Tue, 14 Apr 2020 21:30:12 GMT  
		Size: 996.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3381a8a42899a552e62b60b01a7abbfd6f3eb28a0d55e7c09e3b2d940a3cea74`  
		Last Modified: Tue, 14 Apr 2020 21:30:28 GMT  
		Size: 7.3 KB (7319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e621462fe4eadd3d9466815b3f3a6287f6f2173bbbcf3f6211cfc38a962a633`  
		Last Modified: Tue, 14 Apr 2020 21:30:28 GMT  
		Size: 7.1 MB (7112513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:full`

```console
$ docker pull open-liberty@sha256:f85555cb6679fcc10dde99f291dcea6f96b0a52a4003a9d6ef29f3172bd500d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full` - linux; amd64

```console
$ docker pull open-liberty@sha256:131363ed6037137224bad3e56b37a9f466679865076ae2d737d7b77c81c79678
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.3 MB (252334759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01eb4a28d5b757bfbd3d91834d91adbc680499c52c6635247bdb4c5b35336738`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:37:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:22:51 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 20 Apr 2020 17:23:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Mon, 20 Apr 2020 19:01:15 GMT
ARG OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:01:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Mon, 20 Apr 2020 19:01:15 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Mon, 20 Apr 2020 19:01:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Mon, 20 Apr 2020 19:01:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:01:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 20 Apr 2020 19:01:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Mon, 20 Apr 2020 19:01:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Mon, 20 Apr 2020 19:01:56 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Mon, 20 Apr 2020 19:01:57 GMT
USER 1001
# Mon, 20 Apr 2020 19:01:57 GMT
EXPOSE 9080 9443
# Mon, 20 Apr 2020 19:01:57 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Mon, 20 Apr 2020 19:01:57 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Mon, 20 Apr 2020 19:02:10 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7abfeb06800729d4f24d971e8017c537c4fa86368ae0bca66a7b36ca2b4189`  
		Last Modified: Fri, 20 Mar 2020 19:40:17 GMT  
		Size: 13.3 MB (13325178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ddacaa0d9e81143e1cdfaf134d500ebdc3ea02dd32c6294a4c0666ef29c52`  
		Last Modified: Mon, 20 Apr 2020 17:26:40 GMT  
		Size: 48.5 MB (48502646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e3a198fab752e5bf7ca8c3380756c6e90a617fc95dd350acd499a26e6a0954`  
		Last Modified: Mon, 20 Apr 2020 19:03:58 GMT  
		Size: 6.6 KB (6575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657e17f9073f4820ee1e1c08e88a66d74f86ac3202bfbdd2421014048e6f13b0`  
		Last Modified: Mon, 20 Apr 2020 19:04:15 GMT  
		Size: 155.4 MB (155444332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69689319d8fd691b224bcd663f153f7418d74236de448faec3eee3ed408db46d`  
		Last Modified: Mon, 20 Apr 2020 19:03:57 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172a5609f53c5b0799609963dbff71b62a5921aff1d2173cb4583ae4a32068d`  
		Last Modified: Mon, 20 Apr 2020 19:03:58 GMT  
		Size: 7.5 KB (7483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45180981b6c9e5df07ea7fec898e6ea1fd6da68877c117fe9e9b2bf05a9cdb1c`  
		Last Modified: Mon, 20 Apr 2020 19:04:01 GMT  
		Size: 8.3 MB (8319699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2140f49941f807b0f3e006b4ad3c22678c52945e3ed162cd20b316c339273d`  
		Last Modified: Mon, 20 Apr 2020 19:04:19 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:66b3bfff0ca1a3d67e6ba64a8782ed11c27613cd65e0f964f6a8984448f34390
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254524571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dca468570ba06443203845ba493880137c137a3a6733a841961679d4ec5af7ef`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:22:18 GMT
ADD file:226ecdf321a0fde3bea0d6e88db018b3d077f676a1f1e06942217ebb26a02301 in / 
# Fri, 20 Mar 2020 19:22:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:22:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:22:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:22:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:41:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:44:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:47:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:48:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:48:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:48:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Tue, 14 Apr 2020 21:16:58 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Tue, 14 Apr 2020 21:16:59 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Tue, 14 Apr 2020 21:17:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Tue, 14 Apr 2020 21:17:02 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Tue, 14 Apr 2020 21:17:05 GMT
ARG OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:17:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Tue, 14 Apr 2020 21:17:09 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:18:08 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:18:14 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:18:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:18:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:18:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:19:01 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:19:04 GMT
USER 1001
# Tue, 14 Apr 2020 21:19:06 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:19:10 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:19:11 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Tue, 14 Apr 2020 21:19:27 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:044eae4257f9584af1a24a5cdb9754c96aea36080e68260ddbabab04827bac00`  
		Last Modified: Mon, 16 Mar 2020 15:38:59 GMT  
		Size: 30.4 MB (30399915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf63a142f3acf0fc36d344bc173f2e1990e692aff0c1237ed6dc96cf38cfb2e`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64d9f5f16809d964026266c73b1c06d3cc0dc517437a91d8639758b80958679`  
		Last Modified: Fri, 20 Mar 2020 19:25:01 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c34444f41441c2f598f5dda94ec1b47ee527ce6e5025d70e5eea41a400d16b1`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa3d39187779cfab3b684c0f6e3d861528565e584fbb8dc2e72d633644f21c`  
		Last Modified: Fri, 20 Mar 2020 19:52:26 GMT  
		Size: 14.0 MB (13970663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1612cc71117278a0165cc5c3d4ec4b8a4ae0ad0ddb6ec8ad048b3847a9bcd6a`  
		Last Modified: Fri, 20 Mar 2020 19:55:35 GMT  
		Size: 48.4 MB (48421548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010f05b82c7527404fee92090f1a73ced593eb3e02e389ce7b4ba397901b14f0`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d720535de9153a486814f66ac2a1fdd15f6481a1646c6d996c205ef5ecfd9e68`  
		Last Modified: Tue, 14 Apr 2020 21:23:45 GMT  
		Size: 155.4 MB (155444610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26414e36438cdf17f758f69097373b0fa8206ca44057f099ec2baac1c54a96c2`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2189fd264a66b6912fb4d22070ce4ac884f467cb5fb62abf616cb176bb9c4429`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b81cf6e099c845688b3e0466f3e3bc5c2f40268abb19c80084f7b62618b948`  
		Last Modified: Tue, 14 Apr 2020 21:23:32 GMT  
		Size: 6.2 MB (6235447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c182295927dd2271e3c6f5f4d454331c92425c44028878481858c0eb0d437529`  
		Last Modified: Tue, 14 Apr 2020 21:23:58 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; s390x

```console
$ docker pull open-liberty@sha256:f50f3e431d5f2b358093da92c018e5f3427a929bf4839efb303a9e0644716f6d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249240799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab51f3db1bbc3cbd8888456409f75d04f981e0ab1172a3fb6cba820bd65f6a5`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:38:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:38:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:40:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:40:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Tue, 14 Apr 2020 21:28:11 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Tue, 14 Apr 2020 21:28:12 GMT
ARG OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:28:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Tue, 14 Apr 2020 21:28:13 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:28:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:28:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:28:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:28:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:28:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:28:43 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:28:43 GMT
USER 1001
# Tue, 14 Apr 2020 21:28:44 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:28:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:28:44 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Tue, 14 Apr 2020 21:28:52 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c87faf3e6b36db60f122e065a6d270147409d2b806f06443b02248d6187ad`  
		Last Modified: Fri, 20 Mar 2020 19:42:19 GMT  
		Size: 13.0 MB (13043890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1095d74aa4b9db1c93872abb7a2b7b6afc292f944a2827d13f6216bf00d1406a`  
		Last Modified: Fri, 20 Mar 2020 19:44:13 GMT  
		Size: 48.2 MB (48169610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a83aafe706efa527deafaf845f6395f19bec33c30f0181c0e7d9d2028b0ecc`  
		Last Modified: Tue, 14 Apr 2020 21:29:47 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301c8aa77f82e62e030d053a5cbed03cb942bd83b38439a8081b059cbb6c4010`  
		Last Modified: Tue, 14 Apr 2020 21:30:01 GMT  
		Size: 155.4 MB (155443515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9c50f5d435d6d6b8e3bdfd1910cb7d6a551f41d4e06f6b3d1191cf9c465d8c`  
		Last Modified: Tue, 14 Apr 2020 21:29:47 GMT  
		Size: 970.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2871964de904d8b3852ee5fafbbaeb6da1b499c703d16d977289ee12bc688edb`  
		Last Modified: Tue, 14 Apr 2020 21:29:48 GMT  
		Size: 7.6 KB (7573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abda9230c219becac36e973139c3cd34c432f262d02e2b1db5d4091c5ba9bcb`  
		Last Modified: Tue, 14 Apr 2020 21:29:49 GMT  
		Size: 7.2 MB (7165852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e528b7a6e5db49bec70935990d33cb30e88aa67041a3be72594974418fbdc`  
		Last Modified: Tue, 14 Apr 2020 21:30:06 GMT  
		Size: 963.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:full-java8-openj9`

```console
$ docker pull open-liberty@sha256:f85555cb6679fcc10dde99f291dcea6f96b0a52a4003a9d6ef29f3172bd500d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:131363ed6037137224bad3e56b37a9f466679865076ae2d737d7b77c81c79678
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.3 MB (252334759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01eb4a28d5b757bfbd3d91834d91adbc680499c52c6635247bdb4c5b35336738`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:37:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:22:51 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 20 Apr 2020 17:23:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Mon, 20 Apr 2020 19:01:15 GMT
ARG OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:01:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Mon, 20 Apr 2020 19:01:15 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Mon, 20 Apr 2020 19:01:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Mon, 20 Apr 2020 19:01:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:01:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 20 Apr 2020 19:01:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Mon, 20 Apr 2020 19:01:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Mon, 20 Apr 2020 19:01:56 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Mon, 20 Apr 2020 19:01:57 GMT
USER 1001
# Mon, 20 Apr 2020 19:01:57 GMT
EXPOSE 9080 9443
# Mon, 20 Apr 2020 19:01:57 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Mon, 20 Apr 2020 19:01:57 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Mon, 20 Apr 2020 19:02:10 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7abfeb06800729d4f24d971e8017c537c4fa86368ae0bca66a7b36ca2b4189`  
		Last Modified: Fri, 20 Mar 2020 19:40:17 GMT  
		Size: 13.3 MB (13325178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ddacaa0d9e81143e1cdfaf134d500ebdc3ea02dd32c6294a4c0666ef29c52`  
		Last Modified: Mon, 20 Apr 2020 17:26:40 GMT  
		Size: 48.5 MB (48502646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e3a198fab752e5bf7ca8c3380756c6e90a617fc95dd350acd499a26e6a0954`  
		Last Modified: Mon, 20 Apr 2020 19:03:58 GMT  
		Size: 6.6 KB (6575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657e17f9073f4820ee1e1c08e88a66d74f86ac3202bfbdd2421014048e6f13b0`  
		Last Modified: Mon, 20 Apr 2020 19:04:15 GMT  
		Size: 155.4 MB (155444332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69689319d8fd691b224bcd663f153f7418d74236de448faec3eee3ed408db46d`  
		Last Modified: Mon, 20 Apr 2020 19:03:57 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172a5609f53c5b0799609963dbff71b62a5921aff1d2173cb4583ae4a32068d`  
		Last Modified: Mon, 20 Apr 2020 19:03:58 GMT  
		Size: 7.5 KB (7483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45180981b6c9e5df07ea7fec898e6ea1fd6da68877c117fe9e9b2bf05a9cdb1c`  
		Last Modified: Mon, 20 Apr 2020 19:04:01 GMT  
		Size: 8.3 MB (8319699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2140f49941f807b0f3e006b4ad3c22678c52945e3ed162cd20b316c339273d`  
		Last Modified: Mon, 20 Apr 2020 19:04:19 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:66b3bfff0ca1a3d67e6ba64a8782ed11c27613cd65e0f964f6a8984448f34390
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254524571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dca468570ba06443203845ba493880137c137a3a6733a841961679d4ec5af7ef`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:22:18 GMT
ADD file:226ecdf321a0fde3bea0d6e88db018b3d077f676a1f1e06942217ebb26a02301 in / 
# Fri, 20 Mar 2020 19:22:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:22:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:22:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:22:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:41:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:44:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:47:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:48:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:48:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:48:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Tue, 14 Apr 2020 21:16:58 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Tue, 14 Apr 2020 21:16:59 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Tue, 14 Apr 2020 21:17:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Tue, 14 Apr 2020 21:17:02 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Tue, 14 Apr 2020 21:17:05 GMT
ARG OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:17:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Tue, 14 Apr 2020 21:17:09 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:18:08 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:18:14 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:18:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:18:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:18:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:19:01 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:19:04 GMT
USER 1001
# Tue, 14 Apr 2020 21:19:06 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:19:10 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:19:11 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Tue, 14 Apr 2020 21:19:27 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:044eae4257f9584af1a24a5cdb9754c96aea36080e68260ddbabab04827bac00`  
		Last Modified: Mon, 16 Mar 2020 15:38:59 GMT  
		Size: 30.4 MB (30399915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf63a142f3acf0fc36d344bc173f2e1990e692aff0c1237ed6dc96cf38cfb2e`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64d9f5f16809d964026266c73b1c06d3cc0dc517437a91d8639758b80958679`  
		Last Modified: Fri, 20 Mar 2020 19:25:01 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c34444f41441c2f598f5dda94ec1b47ee527ce6e5025d70e5eea41a400d16b1`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa3d39187779cfab3b684c0f6e3d861528565e584fbb8dc2e72d633644f21c`  
		Last Modified: Fri, 20 Mar 2020 19:52:26 GMT  
		Size: 14.0 MB (13970663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1612cc71117278a0165cc5c3d4ec4b8a4ae0ad0ddb6ec8ad048b3847a9bcd6a`  
		Last Modified: Fri, 20 Mar 2020 19:55:35 GMT  
		Size: 48.4 MB (48421548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010f05b82c7527404fee92090f1a73ced593eb3e02e389ce7b4ba397901b14f0`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d720535de9153a486814f66ac2a1fdd15f6481a1646c6d996c205ef5ecfd9e68`  
		Last Modified: Tue, 14 Apr 2020 21:23:45 GMT  
		Size: 155.4 MB (155444610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26414e36438cdf17f758f69097373b0fa8206ca44057f099ec2baac1c54a96c2`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2189fd264a66b6912fb4d22070ce4ac884f467cb5fb62abf616cb176bb9c4429`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b81cf6e099c845688b3e0466f3e3bc5c2f40268abb19c80084f7b62618b948`  
		Last Modified: Tue, 14 Apr 2020 21:23:32 GMT  
		Size: 6.2 MB (6235447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c182295927dd2271e3c6f5f4d454331c92425c44028878481858c0eb0d437529`  
		Last Modified: Tue, 14 Apr 2020 21:23:58 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:f50f3e431d5f2b358093da92c018e5f3427a929bf4839efb303a9e0644716f6d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249240799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab51f3db1bbc3cbd8888456409f75d04f981e0ab1172a3fb6cba820bd65f6a5`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:38:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:38:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:40:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:40:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Tue, 14 Apr 2020 21:28:11 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Tue, 14 Apr 2020 21:28:12 GMT
ARG OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:28:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Tue, 14 Apr 2020 21:28:13 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:28:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:28:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:28:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:28:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:28:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:28:43 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:28:43 GMT
USER 1001
# Tue, 14 Apr 2020 21:28:44 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:28:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:28:44 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Tue, 14 Apr 2020 21:28:52 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c87faf3e6b36db60f122e065a6d270147409d2b806f06443b02248d6187ad`  
		Last Modified: Fri, 20 Mar 2020 19:42:19 GMT  
		Size: 13.0 MB (13043890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1095d74aa4b9db1c93872abb7a2b7b6afc292f944a2827d13f6216bf00d1406a`  
		Last Modified: Fri, 20 Mar 2020 19:44:13 GMT  
		Size: 48.2 MB (48169610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a83aafe706efa527deafaf845f6395f19bec33c30f0181c0e7d9d2028b0ecc`  
		Last Modified: Tue, 14 Apr 2020 21:29:47 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301c8aa77f82e62e030d053a5cbed03cb942bd83b38439a8081b059cbb6c4010`  
		Last Modified: Tue, 14 Apr 2020 21:30:01 GMT  
		Size: 155.4 MB (155443515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9c50f5d435d6d6b8e3bdfd1910cb7d6a551f41d4e06f6b3d1191cf9c465d8c`  
		Last Modified: Tue, 14 Apr 2020 21:29:47 GMT  
		Size: 970.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2871964de904d8b3852ee5fafbbaeb6da1b499c703d16d977289ee12bc688edb`  
		Last Modified: Tue, 14 Apr 2020 21:29:48 GMT  
		Size: 7.6 KB (7573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abda9230c219becac36e973139c3cd34c432f262d02e2b1db5d4091c5ba9bcb`  
		Last Modified: Tue, 14 Apr 2020 21:29:49 GMT  
		Size: 7.2 MB (7165852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e528b7a6e5db49bec70935990d33cb30e88aa67041a3be72594974418fbdc`  
		Last Modified: Tue, 14 Apr 2020 21:30:06 GMT  
		Size: 963.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:kernel`

```console
$ docker pull open-liberty@sha256:cafa2fc9760590b034276daa73786636c7bb0686fdc17ccb759d6645ac89c9fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel` - linux; amd64

```console
$ docker pull open-liberty@sha256:d95c956d379effa62163d60f058c3e8c8418b1851f2ce92af2eb4fae625c861f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.3 MB (252333793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c75935b0c89806f04c83063ff85f6ef65d26099b5b324edf853dd5bd82c600f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:37:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:22:51 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 20 Apr 2020 17:23:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Mon, 20 Apr 2020 19:01:15 GMT
ARG OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:01:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Mon, 20 Apr 2020 19:01:15 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Mon, 20 Apr 2020 19:01:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Mon, 20 Apr 2020 19:01:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:01:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 20 Apr 2020 19:01:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Mon, 20 Apr 2020 19:01:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Mon, 20 Apr 2020 19:01:56 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Mon, 20 Apr 2020 19:01:57 GMT
USER 1001
# Mon, 20 Apr 2020 19:01:57 GMT
EXPOSE 9080 9443
# Mon, 20 Apr 2020 19:01:57 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Mon, 20 Apr 2020 19:01:57 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7abfeb06800729d4f24d971e8017c537c4fa86368ae0bca66a7b36ca2b4189`  
		Last Modified: Fri, 20 Mar 2020 19:40:17 GMT  
		Size: 13.3 MB (13325178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ddacaa0d9e81143e1cdfaf134d500ebdc3ea02dd32c6294a4c0666ef29c52`  
		Last Modified: Mon, 20 Apr 2020 17:26:40 GMT  
		Size: 48.5 MB (48502646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e3a198fab752e5bf7ca8c3380756c6e90a617fc95dd350acd499a26e6a0954`  
		Last Modified: Mon, 20 Apr 2020 19:03:58 GMT  
		Size: 6.6 KB (6575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657e17f9073f4820ee1e1c08e88a66d74f86ac3202bfbdd2421014048e6f13b0`  
		Last Modified: Mon, 20 Apr 2020 19:04:15 GMT  
		Size: 155.4 MB (155444332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69689319d8fd691b224bcd663f153f7418d74236de448faec3eee3ed408db46d`  
		Last Modified: Mon, 20 Apr 2020 19:03:57 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172a5609f53c5b0799609963dbff71b62a5921aff1d2173cb4583ae4a32068d`  
		Last Modified: Mon, 20 Apr 2020 19:03:58 GMT  
		Size: 7.5 KB (7483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45180981b6c9e5df07ea7fec898e6ea1fd6da68877c117fe9e9b2bf05a9cdb1c`  
		Last Modified: Mon, 20 Apr 2020 19:04:01 GMT  
		Size: 8.3 MB (8319699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:885bdbb074840310694a74b14f6874fee1b44a5ae0c8b8ab2eb2dadcb540d29f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254523605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96499ef52baa69cb556b4bf13edda12a284bf797859a51bd525eaba0ea02ca3a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:22:18 GMT
ADD file:226ecdf321a0fde3bea0d6e88db018b3d077f676a1f1e06942217ebb26a02301 in / 
# Fri, 20 Mar 2020 19:22:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:22:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:22:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:22:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:41:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:44:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:47:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:48:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:48:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:48:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Tue, 14 Apr 2020 21:16:58 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Tue, 14 Apr 2020 21:16:59 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Tue, 14 Apr 2020 21:17:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Tue, 14 Apr 2020 21:17:02 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Tue, 14 Apr 2020 21:17:05 GMT
ARG OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:17:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Tue, 14 Apr 2020 21:17:09 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:18:08 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:18:14 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:18:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:18:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:18:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:19:01 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:19:04 GMT
USER 1001
# Tue, 14 Apr 2020 21:19:06 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:19:10 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:19:11 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:044eae4257f9584af1a24a5cdb9754c96aea36080e68260ddbabab04827bac00`  
		Last Modified: Mon, 16 Mar 2020 15:38:59 GMT  
		Size: 30.4 MB (30399915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf63a142f3acf0fc36d344bc173f2e1990e692aff0c1237ed6dc96cf38cfb2e`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64d9f5f16809d964026266c73b1c06d3cc0dc517437a91d8639758b80958679`  
		Last Modified: Fri, 20 Mar 2020 19:25:01 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c34444f41441c2f598f5dda94ec1b47ee527ce6e5025d70e5eea41a400d16b1`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa3d39187779cfab3b684c0f6e3d861528565e584fbb8dc2e72d633644f21c`  
		Last Modified: Fri, 20 Mar 2020 19:52:26 GMT  
		Size: 14.0 MB (13970663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1612cc71117278a0165cc5c3d4ec4b8a4ae0ad0ddb6ec8ad048b3847a9bcd6a`  
		Last Modified: Fri, 20 Mar 2020 19:55:35 GMT  
		Size: 48.4 MB (48421548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010f05b82c7527404fee92090f1a73ced593eb3e02e389ce7b4ba397901b14f0`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d720535de9153a486814f66ac2a1fdd15f6481a1646c6d996c205ef5ecfd9e68`  
		Last Modified: Tue, 14 Apr 2020 21:23:45 GMT  
		Size: 155.4 MB (155444610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26414e36438cdf17f758f69097373b0fa8206ca44057f099ec2baac1c54a96c2`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2189fd264a66b6912fb4d22070ce4ac884f467cb5fb62abf616cb176bb9c4429`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b81cf6e099c845688b3e0466f3e3bc5c2f40268abb19c80084f7b62618b948`  
		Last Modified: Tue, 14 Apr 2020 21:23:32 GMT  
		Size: 6.2 MB (6235447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel` - linux; s390x

```console
$ docker pull open-liberty@sha256:7aa2234775fdf9fd8abed35c76a4857e25436fd0ba1310f0e0e486585001aefa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249239836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897e314a39d705671ceb1d25f21a45eb22951803b135d1f1e06ac00e54110ef4`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:38:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:38:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:40:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:40:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Tue, 14 Apr 2020 21:28:11 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Tue, 14 Apr 2020 21:28:12 GMT
ARG OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:28:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Tue, 14 Apr 2020 21:28:13 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:28:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:28:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:28:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:28:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:28:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:28:43 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:28:43 GMT
USER 1001
# Tue, 14 Apr 2020 21:28:44 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:28:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:28:44 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c87faf3e6b36db60f122e065a6d270147409d2b806f06443b02248d6187ad`  
		Last Modified: Fri, 20 Mar 2020 19:42:19 GMT  
		Size: 13.0 MB (13043890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1095d74aa4b9db1c93872abb7a2b7b6afc292f944a2827d13f6216bf00d1406a`  
		Last Modified: Fri, 20 Mar 2020 19:44:13 GMT  
		Size: 48.2 MB (48169610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a83aafe706efa527deafaf845f6395f19bec33c30f0181c0e7d9d2028b0ecc`  
		Last Modified: Tue, 14 Apr 2020 21:29:47 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301c8aa77f82e62e030d053a5cbed03cb942bd83b38439a8081b059cbb6c4010`  
		Last Modified: Tue, 14 Apr 2020 21:30:01 GMT  
		Size: 155.4 MB (155443515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9c50f5d435d6d6b8e3bdfd1910cb7d6a551f41d4e06f6b3d1191cf9c465d8c`  
		Last Modified: Tue, 14 Apr 2020 21:29:47 GMT  
		Size: 970.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2871964de904d8b3852ee5fafbbaeb6da1b499c703d16d977289ee12bc688edb`  
		Last Modified: Tue, 14 Apr 2020 21:29:48 GMT  
		Size: 7.6 KB (7573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abda9230c219becac36e973139c3cd34c432f262d02e2b1db5d4091c5ba9bcb`  
		Last Modified: Tue, 14 Apr 2020 21:29:49 GMT  
		Size: 7.2 MB (7165852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:kernel-java8-openj9`

```console
$ docker pull open-liberty@sha256:cafa2fc9760590b034276daa73786636c7bb0686fdc17ccb759d6645ac89c9fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:d95c956d379effa62163d60f058c3e8c8418b1851f2ce92af2eb4fae625c861f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.3 MB (252333793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c75935b0c89806f04c83063ff85f6ef65d26099b5b324edf853dd5bd82c600f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:37:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:22:51 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 20 Apr 2020 17:23:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Mon, 20 Apr 2020 19:01:15 GMT
ARG OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:01:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Mon, 20 Apr 2020 19:01:15 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Mon, 20 Apr 2020 19:01:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Mon, 20 Apr 2020 19:01:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:01:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 20 Apr 2020 19:01:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Mon, 20 Apr 2020 19:01:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Mon, 20 Apr 2020 19:01:56 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Mon, 20 Apr 2020 19:01:57 GMT
USER 1001
# Mon, 20 Apr 2020 19:01:57 GMT
EXPOSE 9080 9443
# Mon, 20 Apr 2020 19:01:57 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Mon, 20 Apr 2020 19:01:57 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7abfeb06800729d4f24d971e8017c537c4fa86368ae0bca66a7b36ca2b4189`  
		Last Modified: Fri, 20 Mar 2020 19:40:17 GMT  
		Size: 13.3 MB (13325178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ddacaa0d9e81143e1cdfaf134d500ebdc3ea02dd32c6294a4c0666ef29c52`  
		Last Modified: Mon, 20 Apr 2020 17:26:40 GMT  
		Size: 48.5 MB (48502646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e3a198fab752e5bf7ca8c3380756c6e90a617fc95dd350acd499a26e6a0954`  
		Last Modified: Mon, 20 Apr 2020 19:03:58 GMT  
		Size: 6.6 KB (6575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657e17f9073f4820ee1e1c08e88a66d74f86ac3202bfbdd2421014048e6f13b0`  
		Last Modified: Mon, 20 Apr 2020 19:04:15 GMT  
		Size: 155.4 MB (155444332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69689319d8fd691b224bcd663f153f7418d74236de448faec3eee3ed408db46d`  
		Last Modified: Mon, 20 Apr 2020 19:03:57 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172a5609f53c5b0799609963dbff71b62a5921aff1d2173cb4583ae4a32068d`  
		Last Modified: Mon, 20 Apr 2020 19:03:58 GMT  
		Size: 7.5 KB (7483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45180981b6c9e5df07ea7fec898e6ea1fd6da68877c117fe9e9b2bf05a9cdb1c`  
		Last Modified: Mon, 20 Apr 2020 19:04:01 GMT  
		Size: 8.3 MB (8319699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:885bdbb074840310694a74b14f6874fee1b44a5ae0c8b8ab2eb2dadcb540d29f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254523605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96499ef52baa69cb556b4bf13edda12a284bf797859a51bd525eaba0ea02ca3a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:22:18 GMT
ADD file:226ecdf321a0fde3bea0d6e88db018b3d077f676a1f1e06942217ebb26a02301 in / 
# Fri, 20 Mar 2020 19:22:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:22:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:22:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:22:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:41:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:44:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:47:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:48:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:48:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:48:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Tue, 14 Apr 2020 21:16:58 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Tue, 14 Apr 2020 21:16:59 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Tue, 14 Apr 2020 21:17:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Tue, 14 Apr 2020 21:17:02 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Tue, 14 Apr 2020 21:17:05 GMT
ARG OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:17:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Tue, 14 Apr 2020 21:17:09 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:18:08 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:18:14 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:18:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:18:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:18:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:19:01 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:19:04 GMT
USER 1001
# Tue, 14 Apr 2020 21:19:06 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:19:10 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:19:11 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:044eae4257f9584af1a24a5cdb9754c96aea36080e68260ddbabab04827bac00`  
		Last Modified: Mon, 16 Mar 2020 15:38:59 GMT  
		Size: 30.4 MB (30399915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf63a142f3acf0fc36d344bc173f2e1990e692aff0c1237ed6dc96cf38cfb2e`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64d9f5f16809d964026266c73b1c06d3cc0dc517437a91d8639758b80958679`  
		Last Modified: Fri, 20 Mar 2020 19:25:01 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c34444f41441c2f598f5dda94ec1b47ee527ce6e5025d70e5eea41a400d16b1`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa3d39187779cfab3b684c0f6e3d861528565e584fbb8dc2e72d633644f21c`  
		Last Modified: Fri, 20 Mar 2020 19:52:26 GMT  
		Size: 14.0 MB (13970663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1612cc71117278a0165cc5c3d4ec4b8a4ae0ad0ddb6ec8ad048b3847a9bcd6a`  
		Last Modified: Fri, 20 Mar 2020 19:55:35 GMT  
		Size: 48.4 MB (48421548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010f05b82c7527404fee92090f1a73ced593eb3e02e389ce7b4ba397901b14f0`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d720535de9153a486814f66ac2a1fdd15f6481a1646c6d996c205ef5ecfd9e68`  
		Last Modified: Tue, 14 Apr 2020 21:23:45 GMT  
		Size: 155.4 MB (155444610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26414e36438cdf17f758f69097373b0fa8206ca44057f099ec2baac1c54a96c2`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2189fd264a66b6912fb4d22070ce4ac884f467cb5fb62abf616cb176bb9c4429`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b81cf6e099c845688b3e0466f3e3bc5c2f40268abb19c80084f7b62618b948`  
		Last Modified: Tue, 14 Apr 2020 21:23:32 GMT  
		Size: 6.2 MB (6235447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:7aa2234775fdf9fd8abed35c76a4857e25436fd0ba1310f0e0e486585001aefa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249239836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897e314a39d705671ceb1d25f21a45eb22951803b135d1f1e06ac00e54110ef4`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:38:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:38:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:40:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:40:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Tue, 14 Apr 2020 21:28:11 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Tue, 14 Apr 2020 21:28:12 GMT
ARG OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:28:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Tue, 14 Apr 2020 21:28:13 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:28:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:28:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:28:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:28:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:28:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:28:43 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:28:43 GMT
USER 1001
# Tue, 14 Apr 2020 21:28:44 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:28:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:28:44 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c87faf3e6b36db60f122e065a6d270147409d2b806f06443b02248d6187ad`  
		Last Modified: Fri, 20 Mar 2020 19:42:19 GMT  
		Size: 13.0 MB (13043890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1095d74aa4b9db1c93872abb7a2b7b6afc292f944a2827d13f6216bf00d1406a`  
		Last Modified: Fri, 20 Mar 2020 19:44:13 GMT  
		Size: 48.2 MB (48169610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a83aafe706efa527deafaf845f6395f19bec33c30f0181c0e7d9d2028b0ecc`  
		Last Modified: Tue, 14 Apr 2020 21:29:47 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301c8aa77f82e62e030d053a5cbed03cb942bd83b38439a8081b059cbb6c4010`  
		Last Modified: Tue, 14 Apr 2020 21:30:01 GMT  
		Size: 155.4 MB (155443515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9c50f5d435d6d6b8e3bdfd1910cb7d6a551f41d4e06f6b3d1191cf9c465d8c`  
		Last Modified: Tue, 14 Apr 2020 21:29:47 GMT  
		Size: 970.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2871964de904d8b3852ee5fafbbaeb6da1b499c703d16d977289ee12bc688edb`  
		Last Modified: Tue, 14 Apr 2020 21:29:48 GMT  
		Size: 7.6 KB (7573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abda9230c219becac36e973139c3cd34c432f262d02e2b1db5d4091c5ba9bcb`  
		Last Modified: Tue, 14 Apr 2020 21:29:49 GMT  
		Size: 7.2 MB (7165852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:latest`

```console
$ docker pull open-liberty@sha256:f85555cb6679fcc10dde99f291dcea6f96b0a52a4003a9d6ef29f3172bd500d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:latest` - linux; amd64

```console
$ docker pull open-liberty@sha256:131363ed6037137224bad3e56b37a9f466679865076ae2d737d7b77c81c79678
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.3 MB (252334759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01eb4a28d5b757bfbd3d91834d91adbc680499c52c6635247bdb4c5b35336738`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:37:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:22:51 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 20 Apr 2020 17:23:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Apr 2020 17:23:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Mon, 20 Apr 2020 19:01:14 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Mon, 20 Apr 2020 19:01:15 GMT
ARG OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:01:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Mon, 20 Apr 2020 19:01:15 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Mon, 20 Apr 2020 19:01:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Mon, 20 Apr 2020 19:01:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Mon, 20 Apr 2020 19:01:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 20 Apr 2020 19:01:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Mon, 20 Apr 2020 19:01:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Mon, 20 Apr 2020 19:01:56 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Mon, 20 Apr 2020 19:01:57 GMT
USER 1001
# Mon, 20 Apr 2020 19:01:57 GMT
EXPOSE 9080 9443
# Mon, 20 Apr 2020 19:01:57 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Mon, 20 Apr 2020 19:01:57 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Mon, 20 Apr 2020 19:02:10 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7abfeb06800729d4f24d971e8017c537c4fa86368ae0bca66a7b36ca2b4189`  
		Last Modified: Fri, 20 Mar 2020 19:40:17 GMT  
		Size: 13.3 MB (13325178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ddacaa0d9e81143e1cdfaf134d500ebdc3ea02dd32c6294a4c0666ef29c52`  
		Last Modified: Mon, 20 Apr 2020 17:26:40 GMT  
		Size: 48.5 MB (48502646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e3a198fab752e5bf7ca8c3380756c6e90a617fc95dd350acd499a26e6a0954`  
		Last Modified: Mon, 20 Apr 2020 19:03:58 GMT  
		Size: 6.6 KB (6575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657e17f9073f4820ee1e1c08e88a66d74f86ac3202bfbdd2421014048e6f13b0`  
		Last Modified: Mon, 20 Apr 2020 19:04:15 GMT  
		Size: 155.4 MB (155444332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69689319d8fd691b224bcd663f153f7418d74236de448faec3eee3ed408db46d`  
		Last Modified: Mon, 20 Apr 2020 19:03:57 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172a5609f53c5b0799609963dbff71b62a5921aff1d2173cb4583ae4a32068d`  
		Last Modified: Mon, 20 Apr 2020 19:03:58 GMT  
		Size: 7.5 KB (7483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45180981b6c9e5df07ea7fec898e6ea1fd6da68877c117fe9e9b2bf05a9cdb1c`  
		Last Modified: Mon, 20 Apr 2020 19:04:01 GMT  
		Size: 8.3 MB (8319699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2140f49941f807b0f3e006b4ad3c22678c52945e3ed162cd20b316c339273d`  
		Last Modified: Mon, 20 Apr 2020 19:04:19 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:66b3bfff0ca1a3d67e6ba64a8782ed11c27613cd65e0f964f6a8984448f34390
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254524571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dca468570ba06443203845ba493880137c137a3a6733a841961679d4ec5af7ef`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 19:22:18 GMT
ADD file:226ecdf321a0fde3bea0d6e88db018b3d077f676a1f1e06942217ebb26a02301 in / 
# Fri, 20 Mar 2020 19:22:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:22:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:22:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:22:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:41:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:44:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:47:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:48:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:48:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:48:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Tue, 14 Apr 2020 21:16:58 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Tue, 14 Apr 2020 21:16:59 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Tue, 14 Apr 2020 21:17:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Tue, 14 Apr 2020 21:17:02 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Tue, 14 Apr 2020 21:17:05 GMT
ARG OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:17:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Tue, 14 Apr 2020 21:17:09 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:18:08 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:18:14 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:18:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:18:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:18:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:19:01 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:19:04 GMT
USER 1001
# Tue, 14 Apr 2020 21:19:06 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:19:10 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:19:11 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Tue, 14 Apr 2020 21:19:27 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:044eae4257f9584af1a24a5cdb9754c96aea36080e68260ddbabab04827bac00`  
		Last Modified: Mon, 16 Mar 2020 15:38:59 GMT  
		Size: 30.4 MB (30399915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf63a142f3acf0fc36d344bc173f2e1990e692aff0c1237ed6dc96cf38cfb2e`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64d9f5f16809d964026266c73b1c06d3cc0dc517437a91d8639758b80958679`  
		Last Modified: Fri, 20 Mar 2020 19:25:01 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c34444f41441c2f598f5dda94ec1b47ee527ce6e5025d70e5eea41a400d16b1`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa3d39187779cfab3b684c0f6e3d861528565e584fbb8dc2e72d633644f21c`  
		Last Modified: Fri, 20 Mar 2020 19:52:26 GMT  
		Size: 14.0 MB (13970663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1612cc71117278a0165cc5c3d4ec4b8a4ae0ad0ddb6ec8ad048b3847a9bcd6a`  
		Last Modified: Fri, 20 Mar 2020 19:55:35 GMT  
		Size: 48.4 MB (48421548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010f05b82c7527404fee92090f1a73ced593eb3e02e389ce7b4ba397901b14f0`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d720535de9153a486814f66ac2a1fdd15f6481a1646c6d996c205ef5ecfd9e68`  
		Last Modified: Tue, 14 Apr 2020 21:23:45 GMT  
		Size: 155.4 MB (155444610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26414e36438cdf17f758f69097373b0fa8206ca44057f099ec2baac1c54a96c2`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2189fd264a66b6912fb4d22070ce4ac884f467cb5fb62abf616cb176bb9c4429`  
		Last Modified: Tue, 14 Apr 2020 21:23:31 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b81cf6e099c845688b3e0466f3e3bc5c2f40268abb19c80084f7b62618b948`  
		Last Modified: Tue, 14 Apr 2020 21:23:32 GMT  
		Size: 6.2 MB (6235447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c182295927dd2271e3c6f5f4d454331c92425c44028878481858c0eb0d437529`  
		Last Modified: Tue, 14 Apr 2020 21:23:58 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; s390x

```console
$ docker pull open-liberty@sha256:f50f3e431d5f2b358093da92c018e5f3427a929bf4839efb303a9e0644716f6d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249240799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab51f3db1bbc3cbd8888456409f75d04f981e0ab1172a3fb6cba820bd65f6a5`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:38:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:38:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:40:26 GMT
ENV JAVA_VERSION=jdk8u242-b08_openj9-0.18.1
# Fri, 20 Mar 2020 19:40:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='438cd1be6a3396d102482f6c2f77cf1146aa38ec866f7bc82739fa77cd172be0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_ppc64le_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        s390x)          ESUM='9b11232cbffcd8fd243f6340ef7cc73ce37c437c66522c19e24d548a7e87b075';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_s390x_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        amd64|x86_64)          ESUM='985d3134b64c6196d4c9ddbc87af0c62b0e643cef71b29f3d25a8c7811811745';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08_openj9-0.18.1/OpenJDK8U-jre_x64_linux_openj9_8u242b08_openj9-0.18.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:40:46 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Tue, 14 Apr 2020 21:28:11 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Tue, 14 Apr 2020 21:28:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Tue, 14 Apr 2020 21:28:12 GMT
ARG OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:28:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714
# Tue, 14 Apr 2020 21:28:13 GMT
COPY dir:288d876eaccdd384bd75c6772f2b17f9dfa7b09f99bd44ed4b8e11f94b366e25 in /opt/ol/helpers 
# Tue, 14 Apr 2020 21:28:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 14 Apr 2020 21:28:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 14 Apr 2020 21:28:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 14 Apr 2020 21:28:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 14 Apr 2020 21:28:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 14 Apr 2020 21:28:43 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Tue, 14 Apr 2020 21:28:43 GMT
USER 1001
# Tue, 14 Apr 2020 21:28:44 GMT
EXPOSE 9080 9443
# Tue, 14 Apr 2020 21:28:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 14 Apr 2020 21:28:44 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Tue, 14 Apr 2020 21:28:52 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c87faf3e6b36db60f122e065a6d270147409d2b806f06443b02248d6187ad`  
		Last Modified: Fri, 20 Mar 2020 19:42:19 GMT  
		Size: 13.0 MB (13043890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1095d74aa4b9db1c93872abb7a2b7b6afc292f944a2827d13f6216bf00d1406a`  
		Last Modified: Fri, 20 Mar 2020 19:44:13 GMT  
		Size: 48.2 MB (48169610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a83aafe706efa527deafaf845f6395f19bec33c30f0181c0e7d9d2028b0ecc`  
		Last Modified: Tue, 14 Apr 2020 21:29:47 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301c8aa77f82e62e030d053a5cbed03cb942bd83b38439a8081b059cbb6c4010`  
		Last Modified: Tue, 14 Apr 2020 21:30:01 GMT  
		Size: 155.4 MB (155443515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9c50f5d435d6d6b8e3bdfd1910cb7d6a551f41d4e06f6b3d1191cf9c465d8c`  
		Last Modified: Tue, 14 Apr 2020 21:29:47 GMT  
		Size: 970.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2871964de904d8b3852ee5fafbbaeb6da1b499c703d16d977289ee12bc688edb`  
		Last Modified: Tue, 14 Apr 2020 21:29:48 GMT  
		Size: 7.6 KB (7573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abda9230c219becac36e973139c3cd34c432f262d02e2b1db5d4091c5ba9bcb`  
		Last Modified: Tue, 14 Apr 2020 21:29:49 GMT  
		Size: 7.2 MB (7165852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e528b7a6e5db49bec70935990d33cb30e88aa67041a3be72594974418fbdc`  
		Last Modified: Tue, 14 Apr 2020 21:30:06 GMT  
		Size: 963.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
