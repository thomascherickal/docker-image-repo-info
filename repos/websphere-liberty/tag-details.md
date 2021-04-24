<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `websphere-liberty`

-	[`websphere-liberty:20.0.0.12-full-java11-openj9`](#websphere-liberty200012-full-java11-openj9)
-	[`websphere-liberty:20.0.0.12-full-java8-ibmjava`](#websphere-liberty200012-full-java8-ibmjava)
-	[`websphere-liberty:20.0.0.12-kernel-java11-openj9`](#websphere-liberty200012-kernel-java11-openj9)
-	[`websphere-liberty:20.0.0.12-kernel-java8-ibmjava`](#websphere-liberty200012-kernel-java8-ibmjava)
-	[`websphere-liberty:21.0.0.3-full-java11-openj9`](#websphere-liberty21003-full-java11-openj9)
-	[`websphere-liberty:21.0.0.3-full-java8-ibmjava`](#websphere-liberty21003-full-java8-ibmjava)
-	[`websphere-liberty:21.0.0.3-kernel-java11-openj9`](#websphere-liberty21003-kernel-java11-openj9)
-	[`websphere-liberty:21.0.0.3-kernel-java8-ibmjava`](#websphere-liberty21003-kernel-java8-ibmjava)
-	[`websphere-liberty:21.0.0.4-full-java11-openj9`](#websphere-liberty21004-full-java11-openj9)
-	[`websphere-liberty:21.0.0.4-full-java8-ibmjava`](#websphere-liberty21004-full-java8-ibmjava)
-	[`websphere-liberty:21.0.0.4-kernel-java11-openj9`](#websphere-liberty21004-kernel-java11-openj9)
-	[`websphere-liberty:21.0.0.4-kernel-java8-ibmjava`](#websphere-liberty21004-kernel-java8-ibmjava)
-	[`websphere-liberty:full`](#websphere-libertyfull)
-	[`websphere-liberty:full-java11-openj9`](#websphere-libertyfull-java11-openj9)
-	[`websphere-liberty:kernel`](#websphere-libertykernel)
-	[`websphere-liberty:kernel-java11-openj9`](#websphere-libertykernel-java11-openj9)
-	[`websphere-liberty:latest`](#websphere-libertylatest)

## `websphere-liberty:20.0.0.12-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:9859e49fa863504abc1d20ba1267d30bfe3bcca391a6e1fec3e730e95368220e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:20.0.0.12-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:49aa464afb2c2d7e3af705fa95df60d73e4e2a8920eb168b32286e534d155d66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.3 MB (316279108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ddf0ea4cc63b052194e75c8fb196a9dcdcef4fca959000a5194793d2a8ca72`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 01:29:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 01:29:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:32:52 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:10 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 21:40:48 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:40:48 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:52:45 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Thu, 22 Apr 2021 21:52:45 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Thu, 22 Apr 2021 21:52:45 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Thu, 22 Apr 2021 21:52:46 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:52:46 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Thu, 22 Apr 2021 21:52:46 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:52:46 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:52:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:52:54 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:52:54 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Thu, 22 Apr 2021 21:52:55 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:52:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:52:56 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:52:56 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:52:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:53:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:53:05 GMT
ENV RANDFILE=/tmp/.rnd
# Thu, 22 Apr 2021 21:53:05 GMT
USER 1001
# Thu, 22 Apr 2021 21:53:05 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:53:05 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:53:06 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 21:53:13 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:53:13 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 21:55:54 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 21:55:55 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 21:56:29 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04b772c31f76720583412a2507c5c53889985db45169a85f0d3cd7f842e041a`  
		Last Modified: Sat, 03 Apr 2021 01:39:30 GMT  
		Size: 16.0 MB (16032891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf71362343a962febc8c6ce8c4fd12d961c5712407993471f60ac0e5d43415e`  
		Last Modified: Mon, 19 Apr 2021 18:30:17 GMT  
		Size: 42.4 MB (42440313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9163852ff25e45c3b95c7b759a719b91afa29724136e68d1cf7f822c034c4df`  
		Last Modified: Mon, 19 Apr 2021 18:30:04 GMT  
		Size: 4.0 MB (4025359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf4544075da5a2c6e7e1b2994b4e7636ccfe9b195b9bb20633733c96ec9a4f9`  
		Last Modified: Thu, 22 Apr 2021 21:59:06 GMT  
		Size: 14.1 MB (14073296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc613cdafc1c7638c8e6e19a98b47464b53ed0758b32961a8ac7780be065560`  
		Last Modified: Thu, 22 Apr 2021 21:59:01 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1783f70e1fa5a4b6784678ac26ee301431e1fd49ab67ec6d1c5670bf1f3fbb16`  
		Last Modified: Thu, 22 Apr 2021 21:59:01 GMT  
		Size: 9.5 KB (9544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774ae461e99f7b8733efbb61a4690422357faa1c019ba98c32119eebd94a8e52`  
		Last Modified: Thu, 22 Apr 2021 21:59:01 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a0fcd773f7170f8b6ecd93b521d77d68777a7041eebbf8ce5d6d7b3fd5318c`  
		Last Modified: Thu, 22 Apr 2021 21:59:01 GMT  
		Size: 10.5 KB (10528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7315afa7e7544b7a663e1baa7146a4cd1bb0d2b26e6bf855b9d7a18fe3dfbf`  
		Last Modified: Thu, 22 Apr 2021 21:59:02 GMT  
		Size: 2.5 MB (2488744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc49043520d0ff26d0907a5bba87aed2572f3f24eb8e540be369d54aef6eb62a`  
		Last Modified: Thu, 22 Apr 2021 21:59:30 GMT  
		Size: 194.6 MB (194615911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdde7a1ddc9aa91231ca742449789475ca92bb7fb964ca5ac7e6f42157c0ee1`  
		Last Modified: Thu, 22 Apr 2021 21:59:15 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3edd9c6c0a9893eaab32a11827fef2579d405fadf7a13469f099c9d6df369b5`  
		Last Modified: Thu, 22 Apr 2021 21:59:17 GMT  
		Size: 14.0 MB (14010556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.12-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:7ae7d6d28c550c364c55de6921797dcbb0643cfab83fc6a9c2780d2f158efe76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.4 MB (320423624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40ac3aa03e2e2f132e2e68f7eadf2f5335e863aec0cf1b36a4972d577ff7c7e6`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 05:41:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 05:43:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 05:51:38 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:15 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 22:40:19 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:40:26 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 23:04:58 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Thu, 22 Apr 2021 23:05:07 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Thu, 22 Apr 2021 23:05:12 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Thu, 22 Apr 2021 23:05:14 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 23:05:16 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Thu, 22 Apr 2021 23:05:18 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 23:05:21 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 23:05:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 23:06:01 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 23:06:04 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Thu, 22 Apr 2021 23:06:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 23:06:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 23:06:20 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 23:06:21 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 23:06:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 23:06:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 23:07:02 GMT
ENV RANDFILE=/tmp/.rnd
# Thu, 22 Apr 2021 23:07:07 GMT
USER 1001
# Thu, 22 Apr 2021 23:07:12 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 23:07:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 23:07:23 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 23:07:42 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 23:07:48 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 23:11:11 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 23:11:21 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 23:12:27 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3147f9d7021e4b4f874d531cd0d820bd489543f00c894d4d9df8f2c1b0777d2b`  
		Last Modified: Sat, 03 Apr 2021 06:01:07 GMT  
		Size: 17.2 MB (17208203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422c588ac4abf48f1a915be1f8f943b1dbc48565bc9f3816ef2bc82f6eb2b9e9`  
		Last Modified: Mon, 19 Apr 2021 18:33:46 GMT  
		Size: 43.3 MB (43277555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e121c025bd5ea767e5c45ee767dc2033229a9d9fb8d83a441bd012a380fd`  
		Last Modified: Mon, 19 Apr 2021 18:33:34 GMT  
		Size: 3.3 MB (3280395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b66ce27f9146ef28d689a9a7837de30425440f51f67aa5f45dcb259ade5b3a1`  
		Last Modified: Thu, 22 Apr 2021 23:15:34 GMT  
		Size: 14.1 MB (14074123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a30e1d3bb791d0721eddf551c119e3f3089a3a5fcc30d141ec09fb76cef99a`  
		Last Modified: Thu, 22 Apr 2021 23:15:29 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db08bcff64149d7af98e4d56c1e5658c2334265bd9dd649d3b832ea4a7a65d12`  
		Last Modified: Thu, 22 Apr 2021 23:15:29 GMT  
		Size: 9.6 KB (9551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a56492a0574bd5ef6ffb492e2750f34bbff3f52b54c9fc12ca2d397c5102440`  
		Last Modified: Thu, 22 Apr 2021 23:15:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7827cc282be90661b0fefc8baa7ef2b6b1ef886bea8f78c65ba3916888d7512`  
		Last Modified: Thu, 22 Apr 2021 23:15:29 GMT  
		Size: 10.5 KB (10533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7608bee4598c7a1be1f7cbc80b32f164912322ff73bef3dfdce7058380b29f0f`  
		Last Modified: Thu, 22 Apr 2021 23:15:30 GMT  
		Size: 2.4 MB (2422726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5712f4bea7affbedd308bfa9199bb1ca00d5afacf529b8e92d3c1b6fd60560`  
		Last Modified: Thu, 22 Apr 2021 23:16:02 GMT  
		Size: 194.6 MB (194615922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb71fc7e33dda8f67116699d1c12a170e0fb0627e5f2d8353948a83be03aff7d`  
		Last Modified: Thu, 22 Apr 2021 23:15:42 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a926a9e3116505aa2ee926b60652ea1f41cdf21111cd2b2a612472bce4d74a8a`  
		Last Modified: Thu, 22 Apr 2021 23:15:46 GMT  
		Size: 12.2 MB (12241632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.12-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:f823274b222c18aa9bc7e19f53b27251773c4f6d57c76558c63991f39b71ce69
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.4 MB (313435528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30485c3ca716f34affb573b50fc116333177044889fe27adc418d63879b3ece9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:03:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 22:04:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:10:11 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Fri, 23 Apr 2021 22:11:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 23 Apr 2021 22:11:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 22:11:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 23 Apr 2021 22:12:20 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 23 Apr 2021 23:17:55 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:17:56 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:42:47 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Fri, 23 Apr 2021 23:42:48 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Fri, 23 Apr 2021 23:42:48 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Fri, 23 Apr 2021 23:42:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:42:49 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Fri, 23 Apr 2021 23:42:50 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:42:50 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:43:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:43:07 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:43:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Fri, 23 Apr 2021 23:43:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:43:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:43:10 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:43:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:43:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:43:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:43:25 GMT
ENV RANDFILE=/tmp/.rnd
# Fri, 23 Apr 2021 23:43:26 GMT
USER 1001
# Fri, 23 Apr 2021 23:43:27 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:43:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:43:28 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 23 Apr 2021 23:48:29 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:48:29 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 23 Apr 2021 23:52:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 23 Apr 2021 23:52:21 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 23 Apr 2021 23:53:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bab416938acf6dd045c9fc9097e5768c61b5899b07d110ab3844f447e12b113`  
		Last Modified: Fri, 23 Apr 2021 22:19:05 GMT  
		Size: 15.7 MB (15741779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0273d3bc7cd55960a36b00d19e8d51f8bbeed03d24fd8d551c957fc19ef079b`  
		Last Modified: Fri, 23 Apr 2021 22:22:19 GMT  
		Size: 42.0 MB (41951613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95422aa686364d2877a279281f6eb1157805fa8516aa976b06ce8889dc9f932`  
		Last Modified: Fri, 23 Apr 2021 22:22:13 GMT  
		Size: 3.8 MB (3836026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14990fd09b16cce85a67e70a4e36d5d7ef545bc5829d4dc06518ea0903f4358`  
		Last Modified: Fri, 23 Apr 2021 23:56:06 GMT  
		Size: 14.1 MB (14073762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aa8db5d764898076adcec4d5fcb6d26084791113dbda57be0b413f0ac4ea5a`  
		Last Modified: Fri, 23 Apr 2021 23:56:03 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7e6711cc2aa475abf04587896ab39969dc660ddb9421d972c056ef7b5c5dc2`  
		Last Modified: Fri, 23 Apr 2021 23:56:03 GMT  
		Size: 9.5 KB (9547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe14ed65b3cf26bd582e4bd1eb693e3f71699e9e92311a838656193a9e2477b`  
		Last Modified: Fri, 23 Apr 2021 23:56:03 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73018234e80a68db6be5395e2a277fff7a9f1af426031715465df02238c7249e`  
		Last Modified: Fri, 23 Apr 2021 23:56:03 GMT  
		Size: 10.5 KB (10539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ce511ea4a40133df08b1bc9befe2d7e56b51ab317b52c4a1aa57e2a1b0347`  
		Last Modified: Fri, 23 Apr 2021 23:56:03 GMT  
		Size: 2.5 MB (2456182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65f16c41028a74817e6ad6bfcbc77333a5352ac0b213f3ec5ae985b4adc6863`  
		Last Modified: Fri, 23 Apr 2021 23:56:40 GMT  
		Size: 194.6 MB (194616382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53733f5dce7b155495e96e49df8e86a805c2643b277d79f4ea121fbc946b872`  
		Last Modified: Fri, 23 Apr 2021 23:56:32 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727cc458a6da1a2cd1ccfedd3fe7d36bf0a6ccd5e0e97de73f0bfcaa63aed45a`  
		Last Modified: Fri, 23 Apr 2021 23:56:33 GMT  
		Size: 13.6 MB (13600394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:20.0.0.12-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:0b7021955ea41a8b87c515a09ac3c3dc05363fbd6e8bd5d664bf7a480d67b31b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:20.0.0.12-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:e288402fbc22c5f5c3807a168770e277288ba2059e61492d6c5eee110d60aafb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **401.5 MB (401499441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fde0be4d6aa814b6c1137b0da28d2b72f44dade75a07845f52455802144033a2`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:30:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 09:31:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:31:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 09:31:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 09:31:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:31:17 GMT
ARG VERBOSE=false
# Fri, 26 Mar 2021 21:31:18 GMT
ARG OPENJ9_SCC=true
# Fri, 26 Mar 2021 21:40:32 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Fri, 26 Mar 2021 21:40:33 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Fri, 26 Mar 2021 21:40:33 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Fri, 26 Mar 2021 21:40:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 26 Mar 2021 21:40:33 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Fri, 26 Mar 2021 21:40:33 GMT
ARG LIBERTY_URL
# Fri, 26 Mar 2021 21:40:34 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 26 Mar 2021 21:40:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 21:40:45 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 21:40:46 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Fri, 26 Mar 2021 21:40:46 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 26 Mar 2021 21:40:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 26 Mar 2021 21:40:48 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Fri, 26 Mar 2021 21:40:48 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 26 Mar 2021 21:40:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 26 Mar 2021 21:41:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 26 Mar 2021 21:41:04 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:41:04 GMT
USER 1001
# Fri, 26 Mar 2021 21:41:04 GMT
EXPOSE 9080 9443
# Fri, 26 Mar 2021 21:41:04 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 26 Mar 2021 21:41:05 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 26 Mar 2021 21:41:38 GMT
ARG VERBOSE=false
# Fri, 26 Mar 2021 21:41:38 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 26 Mar 2021 21:44:24 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 26 Mar 2021 21:44:24 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 26 Mar 2021 21:45:06 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4764ed71d2900c9874838108e377eb8821088502d5504fadeb080e5dd1a3e65d`  
		Last Modified: Fri, 26 Mar 2021 09:35:47 GMT  
		Size: 3.0 MB (2958415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf5000c541da177b7cfe59bf3ff8cb271529f443ee224bf88989910e9a2abb1`  
		Last Modified: Fri, 26 Mar 2021 09:36:01 GMT  
		Size: 130.8 MB (130805802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40ee7d487dafaadac6979a031a0ebf6012f22c16e40fbe1bd8f10efce0b9c65`  
		Last Modified: Fri, 26 Mar 2021 21:50:42 GMT  
		Size: 14.0 MB (13974218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d7271e1d74576aed28a2bd8d9d204d8710a6ae9b56d7272219c22df6d1ffc8`  
		Last Modified: Fri, 26 Mar 2021 21:50:39 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be684063c168c2aff35e4fb23280fe43601dee7593e3505b7da6739babcda15f`  
		Last Modified: Fri, 26 Mar 2021 21:50:38 GMT  
		Size: 9.5 KB (9549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee88b6cd6ee2df9893637c15b1e02d9553045adb73c9012fa79da341939115`  
		Last Modified: Fri, 26 Mar 2021 21:50:40 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07e52523e231c16607e11a295f6532f04c620e6d8a35cb21b692316bbf009ef`  
		Last Modified: Fri, 26 Mar 2021 21:50:38 GMT  
		Size: 10.5 KB (10534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda582494cd506b03886741b406ca50a1f5f2b64a906e71ba036f4f85ba18d9e`  
		Last Modified: Fri, 26 Mar 2021 21:50:40 GMT  
		Size: 5.6 MB (5626186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25dff5c8795a4876ec943dedb0967b151bd8d9be7224b5677531162811efac0f`  
		Last Modified: Fri, 26 Mar 2021 21:51:20 GMT  
		Size: 200.2 MB (200202832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eec289478ec51c113035877e59e023aaed08605aedaa036a3d648933cf6f128`  
		Last Modified: Fri, 26 Mar 2021 21:51:05 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce67a12bea5a210d5c3a06156c50e006c0d9ca021cdc1a26f5013c5a730756a`  
		Last Modified: Fri, 26 Mar 2021 21:51:12 GMT  
		Size: 21.2 MB (21198171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.12-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:ebb533855897ecc9054ad93c75ec8c499c1e791fa55d271aa115f108194afa51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **401.3 MB (401302644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74e4aca51799a7c7cff6fe38df6c8d6b19cc4475ddca0bc810fb32d43cb5516`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:57:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 14:58:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:58:33 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 14:59:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 14:59:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:07:09 GMT
ARG VERBOSE=false
# Sat, 27 Mar 2021 05:07:11 GMT
ARG OPENJ9_SCC=true
# Sat, 27 Mar 2021 05:23:35 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Sat, 27 Mar 2021 05:23:37 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Sat, 27 Mar 2021 05:23:40 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Sat, 27 Mar 2021 05:23:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 27 Mar 2021 05:23:49 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Sat, 27 Mar 2021 05:23:52 GMT
ARG LIBERTY_URL
# Sat, 27 Mar 2021 05:23:57 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 27 Mar 2021 05:24:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:24:31 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 27 Mar 2021 05:24:33 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Sat, 27 Mar 2021 05:24:35 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 27 Mar 2021 05:24:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 27 Mar 2021 05:24:45 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Sat, 27 Mar 2021 05:24:45 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 27 Mar 2021 05:24:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 27 Mar 2021 05:25:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 27 Mar 2021 05:25:15 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:25:18 GMT
USER 1001
# Sat, 27 Mar 2021 05:25:20 GMT
EXPOSE 9080 9443
# Sat, 27 Mar 2021 05:25:26 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 27 Mar 2021 05:25:31 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 27 Mar 2021 05:27:56 GMT
ARG VERBOSE=false
# Sat, 27 Mar 2021 05:27:58 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 27 Mar 2021 05:31:19 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Sat, 27 Mar 2021 05:31:25 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 27 Mar 2021 05:32:20 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a8b760dceb1369716f09f0677ac6e4c109c24e134a9c883c7e48e1ee0d081`  
		Last Modified: Fri, 26 Mar 2021 15:03:04 GMT  
		Size: 3.1 MB (3082734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c129b1161496dd5f093240bbcc3a8117babb3970d1b268b5ef2a3b583cf288`  
		Last Modified: Fri, 26 Mar 2021 15:03:19 GMT  
		Size: 130.4 MB (130406650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e083a8b85e6274867b85619d32040273b3cac298423a85f2adebe24c154da84`  
		Last Modified: Sat, 27 Mar 2021 05:40:46 GMT  
		Size: 14.0 MB (13975116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c043a24e6547e666d50f157e890dbf052d4cd46fa64124923b8841c0dbe59050`  
		Last Modified: Sat, 27 Mar 2021 05:40:38 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51816ec3997d042ef07ebdc5c50318747b50acfc2dfe68e8ced9c99d42c10641`  
		Last Modified: Sat, 27 Mar 2021 05:40:38 GMT  
		Size: 9.6 KB (9552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc467a18a7213ea61e1042e263eaf8148207993449a7d2a1002124972c5b9e5`  
		Last Modified: Sat, 27 Mar 2021 05:40:38 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f18ad4fce44fe8da6f0993693f638bc282fd6890b91dfc7000096f2e7066c`  
		Last Modified: Sat, 27 Mar 2021 05:40:38 GMT  
		Size: 10.5 KB (10547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5c14b75ef36bb4cc2deb7a10b6093a362bbb6c1f19ee197b597ce2e6b398ee`  
		Last Modified: Sat, 27 Mar 2021 05:40:39 GMT  
		Size: 5.1 MB (5123714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bee744f44f5cc67ee6aede180f47e432a5f4c97b84652d9cc5a4b3d50300a4`  
		Last Modified: Sat, 27 Mar 2021 05:41:29 GMT  
		Size: 199.7 MB (199700711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c14264a6a67cfabdf91b121aa7ecc6b061b4b6a9b2c492164eddf76c06d40f`  
		Last Modified: Sat, 27 Mar 2021 05:41:08 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6eb1bdb6abaf83673bd5d13aa6ea681beb3c167305751a37a054322e98b46fd`  
		Last Modified: Sat, 27 Mar 2021 05:41:17 GMT  
		Size: 18.6 MB (18567397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.12-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:c3ba620ffcffe507805150be6db3dbe7bb2673b1690875bd8c1ccdec87ecab4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.8 MB (397786781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aab8e79b4cda357d7d5e110a6f7962ed7af1c62c8c64dadbc2b124b8115f6c2`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:25:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 23 Apr 2021 22:25:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:25:17 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 23 Apr 2021 22:26:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 23 Apr 2021 22:26:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:16:58 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:16:58 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:41:58 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Fri, 23 Apr 2021 23:41:59 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Fri, 23 Apr 2021 23:42:00 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Fri, 23 Apr 2021 23:42:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:42:01 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Fri, 23 Apr 2021 23:42:01 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:42:02 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:42:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:42:18 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:42:18 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Fri, 23 Apr 2021 23:42:19 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:42:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:42:21 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:42:22 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:42:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:42:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:42:39 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:42:39 GMT
USER 1001
# Fri, 23 Apr 2021 23:42:40 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:42:40 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:42:41 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 23 Apr 2021 23:43:36 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:43:37 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 23 Apr 2021 23:47:22 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 23 Apr 2021 23:47:35 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 23 Apr 2021 23:48:18 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93b87da546ac7aa6705cd2f20bfe70cf04793ac73561e5dd8c579af88754aec`  
		Last Modified: Fri, 23 Apr 2021 22:28:41 GMT  
		Size: 2.7 MB (2676643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268462fc02d2bd9da227784f5f243759923a14cefb3648739ca02e8fa7d63ee7`  
		Last Modified: Fri, 23 Apr 2021 22:28:50 GMT  
		Size: 128.1 MB (128065984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4df10ec61b2e9901491d4f07888d6c128dfbc89ae81370abc047a85d361b573`  
		Last Modified: Fri, 23 Apr 2021 23:55:57 GMT  
		Size: 14.0 MB (13974414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b6dcfa2ac20b90dbdc5c0eca9e30f63ba290ecb24d0a2a7161dfd1698eb9dc`  
		Last Modified: Fri, 23 Apr 2021 23:55:52 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b8e5538da3fede30dc5d6f993e2d935e513e68b67eec3bf34b49992e0c0a28`  
		Last Modified: Fri, 23 Apr 2021 23:55:55 GMT  
		Size: 9.5 KB (9548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986f755a30bd8e1dce1334bec46b1614c36821840b84ef826782f1ff8d8fd247`  
		Last Modified: Fri, 23 Apr 2021 23:55:52 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c4c1e123eb0af1079650d1d318286fe5e4df814ada15c45d58dc31a274cd54`  
		Last Modified: Fri, 23 Apr 2021 23:55:55 GMT  
		Size: 10.5 KB (10534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503e041448d0e036d4d18f56f75d491f9a4492e94731e354db7370afc652015f`  
		Last Modified: Fri, 23 Apr 2021 23:55:53 GMT  
		Size: 5.8 MB (5776530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cca07b4da726863086c9e80efa52bcf0498db17ec4c66510543a8e83ff33ae`  
		Last Modified: Fri, 23 Apr 2021 23:56:23 GMT  
		Size: 200.4 MB (200355463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bf9b5980ecfadb96f1fcf3bcc6967e8e930fcf1e0950628514511ee7e4622a`  
		Last Modified: Fri, 23 Apr 2021 23:56:10 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48303b42988be9dab5c39442053d70969976646d4444669017e816b857e28656`  
		Last Modified: Fri, 23 Apr 2021 23:56:13 GMT  
		Size: 21.6 MB (21561952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:20.0.0.12-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:5980e90d404e799aa1a38e4da31cea48368d62abce40df0c79339a9124ad6ab0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:20.0.0.12-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:517bb85cf121708889127e989c208693965377616ceeeb03ff4f2b1415a7ffa2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107651695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:868de794a5c32cd1f825e1c673450c6f48b44e3db6f6953e2fb4257d04323a34`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 01:29:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 01:29:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:32:52 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:10 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 21:40:48 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:40:48 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:52:45 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Thu, 22 Apr 2021 21:52:45 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Thu, 22 Apr 2021 21:52:45 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Thu, 22 Apr 2021 21:52:46 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:52:46 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Thu, 22 Apr 2021 21:52:46 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:52:46 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:52:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:52:54 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:52:54 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Thu, 22 Apr 2021 21:52:55 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:52:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:52:56 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:52:56 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:52:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:53:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:53:05 GMT
ENV RANDFILE=/tmp/.rnd
# Thu, 22 Apr 2021 21:53:05 GMT
USER 1001
# Thu, 22 Apr 2021 21:53:05 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:53:05 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:53:06 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04b772c31f76720583412a2507c5c53889985db45169a85f0d3cd7f842e041a`  
		Last Modified: Sat, 03 Apr 2021 01:39:30 GMT  
		Size: 16.0 MB (16032891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf71362343a962febc8c6ce8c4fd12d961c5712407993471f60ac0e5d43415e`  
		Last Modified: Mon, 19 Apr 2021 18:30:17 GMT  
		Size: 42.4 MB (42440313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9163852ff25e45c3b95c7b759a719b91afa29724136e68d1cf7f822c034c4df`  
		Last Modified: Mon, 19 Apr 2021 18:30:04 GMT  
		Size: 4.0 MB (4025359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf4544075da5a2c6e7e1b2994b4e7636ccfe9b195b9bb20633733c96ec9a4f9`  
		Last Modified: Thu, 22 Apr 2021 21:59:06 GMT  
		Size: 14.1 MB (14073296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc613cdafc1c7638c8e6e19a98b47464b53ed0758b32961a8ac7780be065560`  
		Last Modified: Thu, 22 Apr 2021 21:59:01 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1783f70e1fa5a4b6784678ac26ee301431e1fd49ab67ec6d1c5670bf1f3fbb16`  
		Last Modified: Thu, 22 Apr 2021 21:59:01 GMT  
		Size: 9.5 KB (9544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774ae461e99f7b8733efbb61a4690422357faa1c019ba98c32119eebd94a8e52`  
		Last Modified: Thu, 22 Apr 2021 21:59:01 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a0fcd773f7170f8b6ecd93b521d77d68777a7041eebbf8ce5d6d7b3fd5318c`  
		Last Modified: Thu, 22 Apr 2021 21:59:01 GMT  
		Size: 10.5 KB (10528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7315afa7e7544b7a663e1baa7146a4cd1bb0d2b26e6bf855b9d7a18fe3dfbf`  
		Last Modified: Thu, 22 Apr 2021 21:59:02 GMT  
		Size: 2.5 MB (2488744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.12-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:45fca6d5c58e0fcf92c7c63e13e3ba427a66614c7681cd2d2fc4b95d7936fb97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113565124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35b25ace2cb32f896872a8e82e7faa2a9098311da181aa4774b38780607db3c2`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 05:41:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 05:43:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 05:51:38 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:15 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 22:40:19 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:40:26 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 23:04:58 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Thu, 22 Apr 2021 23:05:07 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Thu, 22 Apr 2021 23:05:12 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Thu, 22 Apr 2021 23:05:14 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 23:05:16 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Thu, 22 Apr 2021 23:05:18 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 23:05:21 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 23:05:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 23:06:01 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 23:06:04 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Thu, 22 Apr 2021 23:06:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 23:06:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 23:06:20 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 23:06:21 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 23:06:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 23:06:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 23:07:02 GMT
ENV RANDFILE=/tmp/.rnd
# Thu, 22 Apr 2021 23:07:07 GMT
USER 1001
# Thu, 22 Apr 2021 23:07:12 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 23:07:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 23:07:23 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3147f9d7021e4b4f874d531cd0d820bd489543f00c894d4d9df8f2c1b0777d2b`  
		Last Modified: Sat, 03 Apr 2021 06:01:07 GMT  
		Size: 17.2 MB (17208203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422c588ac4abf48f1a915be1f8f943b1dbc48565bc9f3816ef2bc82f6eb2b9e9`  
		Last Modified: Mon, 19 Apr 2021 18:33:46 GMT  
		Size: 43.3 MB (43277555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e121c025bd5ea767e5c45ee767dc2033229a9d9fb8d83a441bd012a380fd`  
		Last Modified: Mon, 19 Apr 2021 18:33:34 GMT  
		Size: 3.3 MB (3280395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b66ce27f9146ef28d689a9a7837de30425440f51f67aa5f45dcb259ade5b3a1`  
		Last Modified: Thu, 22 Apr 2021 23:15:34 GMT  
		Size: 14.1 MB (14074123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a30e1d3bb791d0721eddf551c119e3f3089a3a5fcc30d141ec09fb76cef99a`  
		Last Modified: Thu, 22 Apr 2021 23:15:29 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db08bcff64149d7af98e4d56c1e5658c2334265bd9dd649d3b832ea4a7a65d12`  
		Last Modified: Thu, 22 Apr 2021 23:15:29 GMT  
		Size: 9.6 KB (9551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a56492a0574bd5ef6ffb492e2750f34bbff3f52b54c9fc12ca2d397c5102440`  
		Last Modified: Thu, 22 Apr 2021 23:15:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7827cc282be90661b0fefc8baa7ef2b6b1ef886bea8f78c65ba3916888d7512`  
		Last Modified: Thu, 22 Apr 2021 23:15:29 GMT  
		Size: 10.5 KB (10533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7608bee4598c7a1be1f7cbc80b32f164912322ff73bef3dfdce7058380b29f0f`  
		Last Modified: Thu, 22 Apr 2021 23:15:30 GMT  
		Size: 2.4 MB (2422726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.12-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:cf5f49a62545164e7953f96a232cedae4445c2f5fe7308f023abc84620ecfc5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105217806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:685dcea7a6f0d953adc1be0206a79e39bcf7dfb5b803376cf1dfe9829459fd30`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:03:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 22:04:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:10:11 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Fri, 23 Apr 2021 22:11:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 23 Apr 2021 22:11:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 22:11:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 23 Apr 2021 22:12:20 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 23 Apr 2021 23:17:55 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:17:56 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:42:47 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Fri, 23 Apr 2021 23:42:48 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Fri, 23 Apr 2021 23:42:48 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Fri, 23 Apr 2021 23:42:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:42:49 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Fri, 23 Apr 2021 23:42:50 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:42:50 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:43:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:43:07 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:43:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Fri, 23 Apr 2021 23:43:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:43:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:43:10 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:43:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:43:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:43:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:43:25 GMT
ENV RANDFILE=/tmp/.rnd
# Fri, 23 Apr 2021 23:43:26 GMT
USER 1001
# Fri, 23 Apr 2021 23:43:27 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:43:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:43:28 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bab416938acf6dd045c9fc9097e5768c61b5899b07d110ab3844f447e12b113`  
		Last Modified: Fri, 23 Apr 2021 22:19:05 GMT  
		Size: 15.7 MB (15741779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0273d3bc7cd55960a36b00d19e8d51f8bbeed03d24fd8d551c957fc19ef079b`  
		Last Modified: Fri, 23 Apr 2021 22:22:19 GMT  
		Size: 42.0 MB (41951613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95422aa686364d2877a279281f6eb1157805fa8516aa976b06ce8889dc9f932`  
		Last Modified: Fri, 23 Apr 2021 22:22:13 GMT  
		Size: 3.8 MB (3836026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14990fd09b16cce85a67e70a4e36d5d7ef545bc5829d4dc06518ea0903f4358`  
		Last Modified: Fri, 23 Apr 2021 23:56:06 GMT  
		Size: 14.1 MB (14073762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aa8db5d764898076adcec4d5fcb6d26084791113dbda57be0b413f0ac4ea5a`  
		Last Modified: Fri, 23 Apr 2021 23:56:03 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7e6711cc2aa475abf04587896ab39969dc660ddb9421d972c056ef7b5c5dc2`  
		Last Modified: Fri, 23 Apr 2021 23:56:03 GMT  
		Size: 9.5 KB (9547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe14ed65b3cf26bd582e4bd1eb693e3f71699e9e92311a838656193a9e2477b`  
		Last Modified: Fri, 23 Apr 2021 23:56:03 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73018234e80a68db6be5395e2a277fff7a9f1af426031715465df02238c7249e`  
		Last Modified: Fri, 23 Apr 2021 23:56:03 GMT  
		Size: 10.5 KB (10539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ce511ea4a40133df08b1bc9befe2d7e56b51ab317b52c4a1aa57e2a1b0347`  
		Last Modified: Fri, 23 Apr 2021 23:56:03 GMT  
		Size: 2.5 MB (2456182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:20.0.0.12-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:567afc9f2996ada29b1d168ee9d579c4c0ca820500cfc09aa0d115e924ad9e34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:20.0.0.12-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:0d0ae8155a5bb5941362a2c5b9d85a479e540ea08efd26b26fe1c52271bfb1cb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.1 MB (180097492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b68159b13cedee60e6bbcdced790ec517a99868c5ce2e586fbe12982bf9978c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:30:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 09:31:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:31:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 09:31:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 09:31:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:31:17 GMT
ARG VERBOSE=false
# Fri, 26 Mar 2021 21:31:18 GMT
ARG OPENJ9_SCC=true
# Fri, 26 Mar 2021 21:40:32 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Fri, 26 Mar 2021 21:40:33 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Fri, 26 Mar 2021 21:40:33 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Fri, 26 Mar 2021 21:40:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 26 Mar 2021 21:40:33 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Fri, 26 Mar 2021 21:40:33 GMT
ARG LIBERTY_URL
# Fri, 26 Mar 2021 21:40:34 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 26 Mar 2021 21:40:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 21:40:45 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 21:40:46 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Fri, 26 Mar 2021 21:40:46 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 26 Mar 2021 21:40:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 26 Mar 2021 21:40:48 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Fri, 26 Mar 2021 21:40:48 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 26 Mar 2021 21:40:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 26 Mar 2021 21:41:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 26 Mar 2021 21:41:04 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:41:04 GMT
USER 1001
# Fri, 26 Mar 2021 21:41:04 GMT
EXPOSE 9080 9443
# Fri, 26 Mar 2021 21:41:04 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 26 Mar 2021 21:41:05 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4764ed71d2900c9874838108e377eb8821088502d5504fadeb080e5dd1a3e65d`  
		Last Modified: Fri, 26 Mar 2021 09:35:47 GMT  
		Size: 3.0 MB (2958415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf5000c541da177b7cfe59bf3ff8cb271529f443ee224bf88989910e9a2abb1`  
		Last Modified: Fri, 26 Mar 2021 09:36:01 GMT  
		Size: 130.8 MB (130805802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40ee7d487dafaadac6979a031a0ebf6012f22c16e40fbe1bd8f10efce0b9c65`  
		Last Modified: Fri, 26 Mar 2021 21:50:42 GMT  
		Size: 14.0 MB (13974218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d7271e1d74576aed28a2bd8d9d204d8710a6ae9b56d7272219c22df6d1ffc8`  
		Last Modified: Fri, 26 Mar 2021 21:50:39 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be684063c168c2aff35e4fb23280fe43601dee7593e3505b7da6739babcda15f`  
		Last Modified: Fri, 26 Mar 2021 21:50:38 GMT  
		Size: 9.5 KB (9549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee88b6cd6ee2df9893637c15b1e02d9553045adb73c9012fa79da341939115`  
		Last Modified: Fri, 26 Mar 2021 21:50:40 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07e52523e231c16607e11a295f6532f04c620e6d8a35cb21b692316bbf009ef`  
		Last Modified: Fri, 26 Mar 2021 21:50:38 GMT  
		Size: 10.5 KB (10534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda582494cd506b03886741b406ca50a1f5f2b64a906e71ba036f4f85ba18d9e`  
		Last Modified: Fri, 26 Mar 2021 21:50:40 GMT  
		Size: 5.6 MB (5626186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.12-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:ea0098902ed7f7cbc86ab8cdce857a8afff2b3ad2391280d2eebbbde6f63dc49
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.0 MB (183033588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:229e2a7fafb62c049861f40c1ee2fb1cdf1dfb0befcb3adb52c52ac476f06c3f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:57:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 14:58:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:58:33 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 14:59:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 14:59:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:07:09 GMT
ARG VERBOSE=false
# Sat, 27 Mar 2021 05:07:11 GMT
ARG OPENJ9_SCC=true
# Sat, 27 Mar 2021 05:23:35 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Sat, 27 Mar 2021 05:23:37 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Sat, 27 Mar 2021 05:23:40 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Sat, 27 Mar 2021 05:23:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 27 Mar 2021 05:23:49 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Sat, 27 Mar 2021 05:23:52 GMT
ARG LIBERTY_URL
# Sat, 27 Mar 2021 05:23:57 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 27 Mar 2021 05:24:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:24:31 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 27 Mar 2021 05:24:33 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Sat, 27 Mar 2021 05:24:35 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 27 Mar 2021 05:24:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 27 Mar 2021 05:24:45 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Sat, 27 Mar 2021 05:24:45 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 27 Mar 2021 05:24:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 27 Mar 2021 05:25:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 27 Mar 2021 05:25:15 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:25:18 GMT
USER 1001
# Sat, 27 Mar 2021 05:25:20 GMT
EXPOSE 9080 9443
# Sat, 27 Mar 2021 05:25:26 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 27 Mar 2021 05:25:31 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a8b760dceb1369716f09f0677ac6e4c109c24e134a9c883c7e48e1ee0d081`  
		Last Modified: Fri, 26 Mar 2021 15:03:04 GMT  
		Size: 3.1 MB (3082734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c129b1161496dd5f093240bbcc3a8117babb3970d1b268b5ef2a3b583cf288`  
		Last Modified: Fri, 26 Mar 2021 15:03:19 GMT  
		Size: 130.4 MB (130406650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e083a8b85e6274867b85619d32040273b3cac298423a85f2adebe24c154da84`  
		Last Modified: Sat, 27 Mar 2021 05:40:46 GMT  
		Size: 14.0 MB (13975116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c043a24e6547e666d50f157e890dbf052d4cd46fa64124923b8841c0dbe59050`  
		Last Modified: Sat, 27 Mar 2021 05:40:38 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51816ec3997d042ef07ebdc5c50318747b50acfc2dfe68e8ced9c99d42c10641`  
		Last Modified: Sat, 27 Mar 2021 05:40:38 GMT  
		Size: 9.6 KB (9552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc467a18a7213ea61e1042e263eaf8148207993449a7d2a1002124972c5b9e5`  
		Last Modified: Sat, 27 Mar 2021 05:40:38 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f18ad4fce44fe8da6f0993693f638bc282fd6890b91dfc7000096f2e7066c`  
		Last Modified: Sat, 27 Mar 2021 05:40:38 GMT  
		Size: 10.5 KB (10547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5c14b75ef36bb4cc2deb7a10b6093a362bbb6c1f19ee197b597ce2e6b398ee`  
		Last Modified: Sat, 27 Mar 2021 05:40:39 GMT  
		Size: 5.1 MB (5123714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.12-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:b1c099564582a14945574a91b48a32161989b6895b9f3b8efc0eb67a50b7f143
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.9 MB (175868418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a7aa9e39c1e1480f526d98393b7bf1d7d6d37d0204861b8c2280590daae1fa`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:25:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 23 Apr 2021 22:25:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:25:17 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 23 Apr 2021 22:26:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 23 Apr 2021 22:26:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:16:58 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:16:58 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:41:58 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Fri, 23 Apr 2021 23:41:59 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Fri, 23 Apr 2021 23:42:00 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Fri, 23 Apr 2021 23:42:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:42:01 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Fri, 23 Apr 2021 23:42:01 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:42:02 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:42:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:42:18 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:42:18 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Fri, 23 Apr 2021 23:42:19 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:42:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:42:21 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:42:22 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:42:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:42:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:42:39 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:42:39 GMT
USER 1001
# Fri, 23 Apr 2021 23:42:40 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:42:40 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:42:41 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93b87da546ac7aa6705cd2f20bfe70cf04793ac73561e5dd8c579af88754aec`  
		Last Modified: Fri, 23 Apr 2021 22:28:41 GMT  
		Size: 2.7 MB (2676643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268462fc02d2bd9da227784f5f243759923a14cefb3648739ca02e8fa7d63ee7`  
		Last Modified: Fri, 23 Apr 2021 22:28:50 GMT  
		Size: 128.1 MB (128065984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4df10ec61b2e9901491d4f07888d6c128dfbc89ae81370abc047a85d361b573`  
		Last Modified: Fri, 23 Apr 2021 23:55:57 GMT  
		Size: 14.0 MB (13974414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b6dcfa2ac20b90dbdc5c0eca9e30f63ba290ecb24d0a2a7161dfd1698eb9dc`  
		Last Modified: Fri, 23 Apr 2021 23:55:52 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b8e5538da3fede30dc5d6f993e2d935e513e68b67eec3bf34b49992e0c0a28`  
		Last Modified: Fri, 23 Apr 2021 23:55:55 GMT  
		Size: 9.5 KB (9548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986f755a30bd8e1dce1334bec46b1614c36821840b84ef826782f1ff8d8fd247`  
		Last Modified: Fri, 23 Apr 2021 23:55:52 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c4c1e123eb0af1079650d1d318286fe5e4df814ada15c45d58dc31a274cd54`  
		Last Modified: Fri, 23 Apr 2021 23:55:55 GMT  
		Size: 10.5 KB (10534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503e041448d0e036d4d18f56f75d491f9a4492e94731e354db7370afc652015f`  
		Last Modified: Fri, 23 Apr 2021 23:55:53 GMT  
		Size: 5.8 MB (5776530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.3-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:dab5a196119d5e8798bcc4a7e82ceb22d36b940195d7b1d5093cb24d0ec9e762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.3-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:2f19a41174f8c2c45730c99b71042dfbfef0e96e74815cf702814aa2096638b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.1 MB (329145880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f609fe19aab6f7cd7ef0d88ac12bdecdfc6f55f5b03185ebaec997588ff25b4`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 01:29:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 01:29:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:32:52 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:10 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 21:40:48 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:40:48 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:48:33 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Thu, 22 Apr 2021 21:48:34 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Thu, 22 Apr 2021 21:48:34 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Thu, 22 Apr 2021 21:48:34 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:48:34 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Thu, 22 Apr 2021 21:48:34 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:48:34 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:48:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:48:42 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:48:42 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Thu, 22 Apr 2021 21:48:43 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:48:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:48:44 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:48:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:48:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:48:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:48:53 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 22 Apr 2021 21:48:53 GMT
USER 1001
# Thu, 22 Apr 2021 21:48:53 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:48:53 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:48:54 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 21:49:01 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:49:01 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 21:51:53 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 21:51:54 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 21:52:28 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04b772c31f76720583412a2507c5c53889985db45169a85f0d3cd7f842e041a`  
		Last Modified: Sat, 03 Apr 2021 01:39:30 GMT  
		Size: 16.0 MB (16032891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf71362343a962febc8c6ce8c4fd12d961c5712407993471f60ac0e5d43415e`  
		Last Modified: Mon, 19 Apr 2021 18:30:17 GMT  
		Size: 42.4 MB (42440313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9163852ff25e45c3b95c7b759a719b91afa29724136e68d1cf7f822c034c4df`  
		Last Modified: Mon, 19 Apr 2021 18:30:04 GMT  
		Size: 4.0 MB (4025359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27124d51bbcd34a7b9c5ca77307857ac8826a5df7ce13344b52d08235bba7934`  
		Last Modified: Thu, 22 Apr 2021 21:58:30 GMT  
		Size: 14.1 MB (14086702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66b15db611395228cd150cf79924843344bd047b6c5692257ac61c370fb78bb`  
		Last Modified: Thu, 22 Apr 2021 21:58:27 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f642892e4176b386da852ba7c8ca979b999d1d646d4b70d97c47b14748f74cb`  
		Last Modified: Thu, 22 Apr 2021 21:58:26 GMT  
		Size: 9.6 KB (9552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aca56f0e23052c96ef1a40fdadf3c7745e6a10b4a886dd1b56043e2ef85fec8`  
		Last Modified: Thu, 22 Apr 2021 21:58:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626b91e4928db98bd94286caa519f81552ea1f50b114fd2ab51d9c483e9f1623`  
		Last Modified: Thu, 22 Apr 2021 21:58:26 GMT  
		Size: 10.5 KB (10538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18d0b3c58eef5da06cf3322879d39897408847806b395cfd01b8f80a705a723`  
		Last Modified: Thu, 22 Apr 2021 21:58:26 GMT  
		Size: 2.5 MB (2502138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce80311ac261dcb41a0304bd9d8d10c3b99c9d5435fc94894a877f605341855`  
		Last Modified: Thu, 22 Apr 2021 21:58:52 GMT  
		Size: 207.2 MB (207198736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8675b05603d8b247f99cff034e07c405dbd0a2e12f2a0c1f95393d906c226b12`  
		Last Modified: Thu, 22 Apr 2021 21:58:38 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb3af4c9512944dad516500de58fe33876c3610552cb4a71a42db58bfaff644`  
		Last Modified: Thu, 22 Apr 2021 21:58:41 GMT  
		Size: 14.3 MB (14267694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.3-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:58848565f270d7c5b546475a446aa64db3137c74086ff3ca2de56e6ef2464bad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.1 MB (333106655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6620a227279975966257a7c9a09ef2a1d05743d1bc9b70bea1def54d3beeccfd`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 05:41:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 05:43:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 05:51:38 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:15 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 22:40:19 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:40:26 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:55:56 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Thu, 22 Apr 2021 22:56:01 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Thu, 22 Apr 2021 22:56:04 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Thu, 22 Apr 2021 22:56:07 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 22:56:11 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Thu, 22 Apr 2021 22:56:17 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 22:56:23 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 22:57:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 22:57:24 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 22:57:36 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Thu, 22 Apr 2021 22:57:41 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:58:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 22:58:10 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 22:58:14 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 22:58:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 22:58:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 22:58:58 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 22 Apr 2021 22:59:03 GMT
USER 1001
# Thu, 22 Apr 2021 22:59:12 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 22:59:15 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 22:59:20 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 22:59:46 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:59:52 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 23:03:36 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 23:03:44 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 23:04:46 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3147f9d7021e4b4f874d531cd0d820bd489543f00c894d4d9df8f2c1b0777d2b`  
		Last Modified: Sat, 03 Apr 2021 06:01:07 GMT  
		Size: 17.2 MB (17208203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422c588ac4abf48f1a915be1f8f943b1dbc48565bc9f3816ef2bc82f6eb2b9e9`  
		Last Modified: Mon, 19 Apr 2021 18:33:46 GMT  
		Size: 43.3 MB (43277555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e121c025bd5ea767e5c45ee767dc2033229a9d9fb8d83a441bd012a380fd`  
		Last Modified: Mon, 19 Apr 2021 18:33:34 GMT  
		Size: 3.3 MB (3280395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e402c8b784836229d4a6f23a04fef46be650c86d43441c64cb4627e74e690f`  
		Last Modified: Thu, 22 Apr 2021 23:14:49 GMT  
		Size: 14.1 MB (14087588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba0a7830256efccd41b236b4322e1ffbe205eaabac9df6e5d75e1a9d73b8dc3`  
		Last Modified: Thu, 22 Apr 2021 23:14:44 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ebdb6344ad1be9c1738144870bb58814653d8c34b103acd6b5236dd6301068`  
		Last Modified: Thu, 22 Apr 2021 23:14:43 GMT  
		Size: 9.6 KB (9550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c511d9355a2718938a2a4c3d1498bdc9868266543dc79cfb4d91de955497f6`  
		Last Modified: Thu, 22 Apr 2021 23:14:43 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cf298325a3827d6db21b8055a6d4e6ff85e39cd75a6e9912e42c1c126a6221`  
		Last Modified: Thu, 22 Apr 2021 23:14:43 GMT  
		Size: 10.5 KB (10536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c475cb3fff03d34494a3e548a8ad23bc7705eb84478ff59554999375041f29`  
		Last Modified: Thu, 22 Apr 2021 23:14:44 GMT  
		Size: 2.4 MB (2430987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f767de19ba9a26f0656f2a102f8a8c5e4d5ee6869ff26139dc64416e0ff043`  
		Last Modified: Thu, 22 Apr 2021 23:15:20 GMT  
		Size: 207.2 MB (207197177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba4c9647e38d917d169a5de267119464cfccf9b3e5576a05ad69a5372cf6306`  
		Last Modified: Thu, 22 Apr 2021 23:15:00 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f836274c71e275c888a4793ad169ef6e6b0bdb7fb03f8f43ca12d2d2a0a43826`  
		Last Modified: Thu, 22 Apr 2021 23:15:04 GMT  
		Size: 12.3 MB (12321671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.3-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:94e3bd056686fd88e274f1d0866bf9fa1ea394166f5471d5539f64922e42f0b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.1 MB (326083570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35a6985d189c29379befcdd8b0c2f1806ffdbd5fbb6037931a26c4dea10f053`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:03:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 22:04:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:10:11 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Fri, 23 Apr 2021 22:11:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 23 Apr 2021 22:11:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 22:11:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 23 Apr 2021 22:12:20 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 23 Apr 2021 23:17:55 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:17:56 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:30:46 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Fri, 23 Apr 2021 23:30:46 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Fri, 23 Apr 2021 23:30:47 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Fri, 23 Apr 2021 23:30:48 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:30:48 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Fri, 23 Apr 2021 23:30:49 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:30:50 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:31:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:31:07 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:31:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Fri, 23 Apr 2021 23:31:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:31:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:31:10 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:31:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:31:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:31:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:31:27 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 23 Apr 2021 23:31:28 GMT
USER 1001
# Fri, 23 Apr 2021 23:31:28 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:31:29 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:31:29 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 23 Apr 2021 23:36:50 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:36:50 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 23 Apr 2021 23:40:47 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 23 Apr 2021 23:40:59 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 23 Apr 2021 23:41:41 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bab416938acf6dd045c9fc9097e5768c61b5899b07d110ab3844f447e12b113`  
		Last Modified: Fri, 23 Apr 2021 22:19:05 GMT  
		Size: 15.7 MB (15741779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0273d3bc7cd55960a36b00d19e8d51f8bbeed03d24fd8d551c957fc19ef079b`  
		Last Modified: Fri, 23 Apr 2021 22:22:19 GMT  
		Size: 42.0 MB (41951613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95422aa686364d2877a279281f6eb1157805fa8516aa976b06ce8889dc9f932`  
		Last Modified: Fri, 23 Apr 2021 22:22:13 GMT  
		Size: 3.8 MB (3836026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f4fac1a8aceea217c7fe53bbfc322b60fbc9aa714e55650ace47a05de81069`  
		Last Modified: Fri, 23 Apr 2021 23:54:57 GMT  
		Size: 14.1 MB (14087190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756fea3647fb5e2b8750dbb5e4c2fcf03f89f52b7e5cb55b7606924b2389ca81`  
		Last Modified: Fri, 23 Apr 2021 23:54:54 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fa9033e59f89cbb013c7d832613bab3a656300357cc70b7eade006a8edefce`  
		Last Modified: Fri, 23 Apr 2021 23:54:54 GMT  
		Size: 9.6 KB (9554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f62d4b9f7c9f91f8d9c689ebf626986dd4c2efd6d86ff851bd15bc6183dded0`  
		Last Modified: Fri, 23 Apr 2021 23:54:54 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491f6056574f25428a41b45fd180908c3bcb491ed462310db1dda218415df01c`  
		Last Modified: Fri, 23 Apr 2021 23:54:54 GMT  
		Size: 10.5 KB (10537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df697bb1f00968be2197f2465a5306f2873b7d22664eeb96b49f2a15ce43654d`  
		Last Modified: Fri, 23 Apr 2021 23:54:54 GMT  
		Size: 2.5 MB (2489469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59753a091e4624a995faf14a9f9ff0afcb986c686a48635b1697d46125128b14`  
		Last Modified: Fri, 23 Apr 2021 23:55:42 GMT  
		Size: 207.2 MB (207198908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d5f5c0b23fd673685a77862a45ffd6f44f6f97f9d801c7938c09aa77a3c6b7`  
		Last Modified: Fri, 23 Apr 2021 23:55:29 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7a099266c968226b8409c4aa7536ccc7546b900ff860ebef4cb27010323e18`  
		Last Modified: Fri, 23 Apr 2021 23:55:30 GMT  
		Size: 13.6 MB (13619199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.3-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:3f1788b323e525eaed4f86650b71394765499d910c9d8b399247c9dd69276066
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.3-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:18902eb4619a6c3c50377fd1d4efaa9a4b9d3ec75ff475b1195e60b2b50d2d5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.5 MB (414462047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f29f7bd268928d680dcec8c1ad8666555fcb0ab86c3812f8b5f0765cdf6c8d`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:30:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 09:31:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:31:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 09:31:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 09:31:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:31:17 GMT
ARG VERBOSE=false
# Fri, 26 Mar 2021 21:31:18 GMT
ARG OPENJ9_SCC=true
# Fri, 26 Mar 2021 21:31:18 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Fri, 26 Mar 2021 21:31:18 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Fri, 26 Mar 2021 21:31:18 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Fri, 26 Mar 2021 21:31:18 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 26 Mar 2021 21:31:19 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Fri, 26 Mar 2021 21:31:19 GMT
ARG LIBERTY_URL
# Fri, 26 Mar 2021 21:31:19 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 26 Mar 2021 21:31:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 21:31:33 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 21:31:33 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Fri, 26 Mar 2021 21:31:33 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 26 Mar 2021 21:31:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 26 Mar 2021 21:31:35 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 26 Mar 2021 21:31:35 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 26 Mar 2021 21:31:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 26 Mar 2021 21:31:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 26 Mar 2021 21:31:49 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:31:49 GMT
USER 1001
# Fri, 26 Mar 2021 21:31:49 GMT
EXPOSE 9080 9443
# Fri, 26 Mar 2021 21:31:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 26 Mar 2021 21:31:49 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 26 Mar 2021 21:32:29 GMT
ARG VERBOSE=false
# Fri, 26 Mar 2021 21:32:30 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 26 Mar 2021 21:35:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 26 Mar 2021 21:35:39 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 26 Mar 2021 21:36:24 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4764ed71d2900c9874838108e377eb8821088502d5504fadeb080e5dd1a3e65d`  
		Last Modified: Fri, 26 Mar 2021 09:35:47 GMT  
		Size: 3.0 MB (2958415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf5000c541da177b7cfe59bf3ff8cb271529f443ee224bf88989910e9a2abb1`  
		Last Modified: Fri, 26 Mar 2021 09:36:01 GMT  
		Size: 130.8 MB (130805802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f62ff9f46b7fe8abf21ca3992ddfdba43c9a869ab05da497fd0c961b82bcc8`  
		Last Modified: Fri, 26 Mar 2021 21:49:10 GMT  
		Size: 14.0 MB (13988287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade44e6f5f910e4171dbe956b6f82444a1a0cf77cbb628a3cd3a4e02b91e4a75`  
		Last Modified: Fri, 26 Mar 2021 21:49:06 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e194224da53e4dca0cfb2e746e2dc2780faf558e27fbea8a051bbb1e645412a`  
		Last Modified: Fri, 26 Mar 2021 21:49:05 GMT  
		Size: 9.6 KB (9555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee645bef2bf69d54e107e8f571dd29a3a04a4bc4b3dc86db1e83a1cc15f0be9`  
		Last Modified: Fri, 26 Mar 2021 21:49:05 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7592107637fd3c10cd009e854a974a81b2a2bb14bbfc045924a369d59d3098`  
		Last Modified: Fri, 26 Mar 2021 21:49:05 GMT  
		Size: 10.5 KB (10545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11fedbbde6cf647ecb2604ada8a232f0040986bc0bab990ba49c28482ddc35f4`  
		Last Modified: Fri, 26 Mar 2021 21:49:07 GMT  
		Size: 5.7 MB (5661783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c44f60c1c5e6897a6c8ab173b4552e16708e2bbf180aab829a6e2045fdd2206`  
		Last Modified: Fri, 26 Mar 2021 21:49:44 GMT  
		Size: 212.8 MB (212822107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1023c04b596fcb951bc35f6638adf41d8ba07d1252a26495c71f95cfd17878`  
		Last Modified: Fri, 26 Mar 2021 21:49:30 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4831ae3a88bfff0d766ba60d4f176b42097c5b1d0821d32427611ff49389f89`  
		Last Modified: Fri, 26 Mar 2021 21:49:34 GMT  
		Size: 21.5 MB (21491809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.3-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:14d6d5397027bfe4fa97b96c5b0a8832ead1b350d6a21d42e6b197b06354c46f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.2 MB (414166762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96cd4d1f389645c6cc87b7b4063c0aa4192e4f1bc46be991e671f85c90aa61e3`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:57:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 14:58:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:58:33 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 14:59:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 14:59:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:07:09 GMT
ARG VERBOSE=false
# Sat, 27 Mar 2021 05:07:11 GMT
ARG OPENJ9_SCC=true
# Sat, 27 Mar 2021 05:07:14 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Sat, 27 Mar 2021 05:07:16 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Sat, 27 Mar 2021 05:07:19 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Sat, 27 Mar 2021 05:07:23 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 27 Mar 2021 05:07:25 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Sat, 27 Mar 2021 05:07:28 GMT
ARG LIBERTY_URL
# Sat, 27 Mar 2021 05:07:30 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 27 Mar 2021 05:08:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:08:06 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 27 Mar 2021 05:08:09 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Sat, 27 Mar 2021 05:08:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 27 Mar 2021 05:08:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 27 Mar 2021 05:08:32 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Sat, 27 Mar 2021 05:08:34 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 27 Mar 2021 05:08:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 27 Mar 2021 05:09:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 27 Mar 2021 05:09:27 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:09:35 GMT
USER 1001
# Sat, 27 Mar 2021 05:09:41 GMT
EXPOSE 9080 9443
# Sat, 27 Mar 2021 05:09:44 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 27 Mar 2021 05:09:48 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 27 Mar 2021 05:13:01 GMT
ARG VERBOSE=false
# Sat, 27 Mar 2021 05:13:03 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 27 Mar 2021 05:17:16 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Sat, 27 Mar 2021 05:17:19 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 27 Mar 2021 05:18:22 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a8b760dceb1369716f09f0677ac6e4c109c24e134a9c883c7e48e1ee0d081`  
		Last Modified: Fri, 26 Mar 2021 15:03:04 GMT  
		Size: 3.1 MB (3082734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c129b1161496dd5f093240bbcc3a8117babb3970d1b268b5ef2a3b583cf288`  
		Last Modified: Fri, 26 Mar 2021 15:03:19 GMT  
		Size: 130.4 MB (130406650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c71325e2d5617b9cd85e190ffdf8af663eb9617a1b6eccb340ab9de410d8e8`  
		Last Modified: Sat, 27 Mar 2021 05:38:58 GMT  
		Size: 14.0 MB (13989148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7124e4edcf5e13bc86bb8c43e5f200bd4a5f4510b57eba64f6f7451d46bd03`  
		Last Modified: Sat, 27 Mar 2021 05:38:51 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2088cb3daf47bf90822cb9bc806e51e7ce37ed6cc0c30909bff2fc88385d983b`  
		Last Modified: Sat, 27 Mar 2021 05:38:51 GMT  
		Size: 9.6 KB (9560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf52d46b34ad387623eef0aada894b720e268856356ec1c782d07b5b8f36561b`  
		Last Modified: Sat, 27 Mar 2021 05:38:52 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f72748eb637591c7ed93f76eca5bef63ff2233917f14fe3109f1b46e3a4e3b4`  
		Last Modified: Sat, 27 Mar 2021 05:38:51 GMT  
		Size: 10.5 KB (10535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0006e35e36fce96b51591922551d02cdfe5d95260d86017619492d5e429bbc62`  
		Last Modified: Sat, 27 Mar 2021 05:38:53 GMT  
		Size: 5.2 MB (5239852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002038b9c565ff9631a3ef1c5cb60c92b47804325e714b3465d0e9acb657f039`  
		Last Modified: Sat, 27 Mar 2021 05:39:44 GMT  
		Size: 212.4 MB (212399252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b32cac1c0cb5a61276927e14e63eed297638c597671e12d00db938c134f781`  
		Last Modified: Sat, 27 Mar 2021 05:39:22 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bcebfab179bef310b9bde05ba59210140a8932425b4d855edfa35d8807f304`  
		Last Modified: Sat, 27 Mar 2021 05:39:27 GMT  
		Size: 18.6 MB (18602811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.3-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:ec03093309c98603a416d3ecb6845f4d54dddb5208ca14a9e3ddc233f8960e77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **410.7 MB (410660108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a055c4d5a8b3680d7928b4c804e24d859318e386ac4ec10fe03fc3d124a7f53`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:25:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 23 Apr 2021 22:25:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:25:17 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 23 Apr 2021 22:26:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 23 Apr 2021 22:26:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:16:58 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:16:58 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:29:48 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Fri, 23 Apr 2021 23:29:49 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Fri, 23 Apr 2021 23:29:50 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Fri, 23 Apr 2021 23:29:50 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:29:51 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Fri, 23 Apr 2021 23:29:52 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:29:52 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:30:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:30:10 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:30:11 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Fri, 23 Apr 2021 23:30:11 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:30:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:30:15 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:30:15 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:30:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:30:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:30:32 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:30:33 GMT
USER 1001
# Fri, 23 Apr 2021 23:30:33 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:30:34 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:30:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 23 Apr 2021 23:31:42 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:31:43 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 23 Apr 2021 23:35:45 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 23 Apr 2021 23:36:01 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 23 Apr 2021 23:36:42 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93b87da546ac7aa6705cd2f20bfe70cf04793ac73561e5dd8c579af88754aec`  
		Last Modified: Fri, 23 Apr 2021 22:28:41 GMT  
		Size: 2.7 MB (2676643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268462fc02d2bd9da227784f5f243759923a14cefb3648739ca02e8fa7d63ee7`  
		Last Modified: Fri, 23 Apr 2021 22:28:50 GMT  
		Size: 128.1 MB (128065984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2e27878ce60350be68bbdb3b8ee9cbfde9b111787d0b974a06b8dffadddcbd`  
		Last Modified: Fri, 23 Apr 2021 23:54:49 GMT  
		Size: 14.0 MB (13988524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894cb19fa986a022ad70870257b92d2c0c4fb51aabb232cd0284dacada85fe2`  
		Last Modified: Fri, 23 Apr 2021 23:54:46 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08d76891a169b900915649827dc512feb56f753883fe52981be6f04d736b2f6`  
		Last Modified: Fri, 23 Apr 2021 23:54:46 GMT  
		Size: 9.6 KB (9557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34ee5d8f9435c0ed35bd9d1b5ae402ce58f34113d03dd5a315a826c6cd83b36`  
		Last Modified: Fri, 23 Apr 2021 23:54:46 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300d3fb2439110af45d80a2ddbf132b397feb71fefce3d1f0a596b771fdb90c`  
		Last Modified: Fri, 23 Apr 2021 23:54:47 GMT  
		Size: 10.5 KB (10543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a38e178e857d2811edcaca15881bfc7721e5afa49da3e0557037dfec12a23f`  
		Last Modified: Fri, 23 Apr 2021 23:54:47 GMT  
		Size: 5.8 MB (5848991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b424a8ac9b26bcdac2c714b92bad760cf44182a95956269fb3f0a873be87e547`  
		Last Modified: Fri, 23 Apr 2021 23:55:15 GMT  
		Size: 213.0 MB (213010696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d93757514d2ad41bbfdd187dc542cb9353de5290ab8d5acda3d7e85435fca`  
		Last Modified: Fri, 23 Apr 2021 23:55:02 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd4875bb40fed31bff06329f774ad259835e6b45dc6c967fed0cdcd164fab27`  
		Last Modified: Fri, 23 Apr 2021 23:55:04 GMT  
		Size: 21.7 MB (21693461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.3-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:8572afa178b89952b55c6c3e25b410344084ad2198638fc3fd7008277f27cba6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.3-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:fc39abe3376b11a33b27b0ea6a93bb4dfa82b2a8c22b61d16b102fd91a396fd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107678507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cd0e8588bf66acce2efe2ec9d8f46bf79a8162e5e496d58646fc734d7763d85`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 01:29:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 01:29:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:32:52 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:10 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 21:40:48 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:40:48 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:48:33 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Thu, 22 Apr 2021 21:48:34 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Thu, 22 Apr 2021 21:48:34 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Thu, 22 Apr 2021 21:48:34 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:48:34 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Thu, 22 Apr 2021 21:48:34 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:48:34 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:48:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:48:42 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:48:42 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Thu, 22 Apr 2021 21:48:43 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:48:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:48:44 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:48:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:48:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:48:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:48:53 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 22 Apr 2021 21:48:53 GMT
USER 1001
# Thu, 22 Apr 2021 21:48:53 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:48:53 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:48:54 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04b772c31f76720583412a2507c5c53889985db45169a85f0d3cd7f842e041a`  
		Last Modified: Sat, 03 Apr 2021 01:39:30 GMT  
		Size: 16.0 MB (16032891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf71362343a962febc8c6ce8c4fd12d961c5712407993471f60ac0e5d43415e`  
		Last Modified: Mon, 19 Apr 2021 18:30:17 GMT  
		Size: 42.4 MB (42440313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9163852ff25e45c3b95c7b759a719b91afa29724136e68d1cf7f822c034c4df`  
		Last Modified: Mon, 19 Apr 2021 18:30:04 GMT  
		Size: 4.0 MB (4025359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27124d51bbcd34a7b9c5ca77307857ac8826a5df7ce13344b52d08235bba7934`  
		Last Modified: Thu, 22 Apr 2021 21:58:30 GMT  
		Size: 14.1 MB (14086702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66b15db611395228cd150cf79924843344bd047b6c5692257ac61c370fb78bb`  
		Last Modified: Thu, 22 Apr 2021 21:58:27 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f642892e4176b386da852ba7c8ca979b999d1d646d4b70d97c47b14748f74cb`  
		Last Modified: Thu, 22 Apr 2021 21:58:26 GMT  
		Size: 9.6 KB (9552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aca56f0e23052c96ef1a40fdadf3c7745e6a10b4a886dd1b56043e2ef85fec8`  
		Last Modified: Thu, 22 Apr 2021 21:58:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626b91e4928db98bd94286caa519f81552ea1f50b114fd2ab51d9c483e9f1623`  
		Last Modified: Thu, 22 Apr 2021 21:58:26 GMT  
		Size: 10.5 KB (10538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18d0b3c58eef5da06cf3322879d39897408847806b395cfd01b8f80a705a723`  
		Last Modified: Thu, 22 Apr 2021 21:58:26 GMT  
		Size: 2.5 MB (2502138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.3-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:f729df932b939ad8f0bb076d39f0caa0d649694f81a32f33a31c145e2228de78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113586856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a25ac2e1f92640f8f556da49f90a38e6680dccfc5c21a6796bca0b5d11a8b338`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 05:41:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 05:43:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 05:51:38 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:15 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 22:40:19 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:40:26 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:55:56 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Thu, 22 Apr 2021 22:56:01 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Thu, 22 Apr 2021 22:56:04 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Thu, 22 Apr 2021 22:56:07 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 22:56:11 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Thu, 22 Apr 2021 22:56:17 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 22:56:23 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 22:57:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 22:57:24 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 22:57:36 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Thu, 22 Apr 2021 22:57:41 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:58:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 22:58:10 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 22:58:14 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 22:58:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 22:58:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 22:58:58 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 22 Apr 2021 22:59:03 GMT
USER 1001
# Thu, 22 Apr 2021 22:59:12 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 22:59:15 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 22:59:20 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3147f9d7021e4b4f874d531cd0d820bd489543f00c894d4d9df8f2c1b0777d2b`  
		Last Modified: Sat, 03 Apr 2021 06:01:07 GMT  
		Size: 17.2 MB (17208203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422c588ac4abf48f1a915be1f8f943b1dbc48565bc9f3816ef2bc82f6eb2b9e9`  
		Last Modified: Mon, 19 Apr 2021 18:33:46 GMT  
		Size: 43.3 MB (43277555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e121c025bd5ea767e5c45ee767dc2033229a9d9fb8d83a441bd012a380fd`  
		Last Modified: Mon, 19 Apr 2021 18:33:34 GMT  
		Size: 3.3 MB (3280395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e402c8b784836229d4a6f23a04fef46be650c86d43441c64cb4627e74e690f`  
		Last Modified: Thu, 22 Apr 2021 23:14:49 GMT  
		Size: 14.1 MB (14087588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba0a7830256efccd41b236b4322e1ffbe205eaabac9df6e5d75e1a9d73b8dc3`  
		Last Modified: Thu, 22 Apr 2021 23:14:44 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ebdb6344ad1be9c1738144870bb58814653d8c34b103acd6b5236dd6301068`  
		Last Modified: Thu, 22 Apr 2021 23:14:43 GMT  
		Size: 9.6 KB (9550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c511d9355a2718938a2a4c3d1498bdc9868266543dc79cfb4d91de955497f6`  
		Last Modified: Thu, 22 Apr 2021 23:14:43 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cf298325a3827d6db21b8055a6d4e6ff85e39cd75a6e9912e42c1c126a6221`  
		Last Modified: Thu, 22 Apr 2021 23:14:43 GMT  
		Size: 10.5 KB (10536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c475cb3fff03d34494a3e548a8ad23bc7705eb84478ff59554999375041f29`  
		Last Modified: Thu, 22 Apr 2021 23:14:44 GMT  
		Size: 2.4 MB (2430987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.3-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0737828b881ffc978313a472df0f167f3230bb616aff887d83285b9835144491
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105264517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b35f835c2859721d78c892a578760dbc2d0d1175ddf1420085542b3855ce38e1`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:03:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 22:04:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:10:11 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Fri, 23 Apr 2021 22:11:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 23 Apr 2021 22:11:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 22:11:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 23 Apr 2021 22:12:20 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 23 Apr 2021 23:17:55 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:17:56 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:30:46 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Fri, 23 Apr 2021 23:30:46 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Fri, 23 Apr 2021 23:30:47 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Fri, 23 Apr 2021 23:30:48 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:30:48 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Fri, 23 Apr 2021 23:30:49 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:30:50 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:31:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:31:07 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:31:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Fri, 23 Apr 2021 23:31:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:31:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:31:10 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:31:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:31:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:31:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:31:27 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 23 Apr 2021 23:31:28 GMT
USER 1001
# Fri, 23 Apr 2021 23:31:28 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:31:29 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:31:29 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bab416938acf6dd045c9fc9097e5768c61b5899b07d110ab3844f447e12b113`  
		Last Modified: Fri, 23 Apr 2021 22:19:05 GMT  
		Size: 15.7 MB (15741779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0273d3bc7cd55960a36b00d19e8d51f8bbeed03d24fd8d551c957fc19ef079b`  
		Last Modified: Fri, 23 Apr 2021 22:22:19 GMT  
		Size: 42.0 MB (41951613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95422aa686364d2877a279281f6eb1157805fa8516aa976b06ce8889dc9f932`  
		Last Modified: Fri, 23 Apr 2021 22:22:13 GMT  
		Size: 3.8 MB (3836026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f4fac1a8aceea217c7fe53bbfc322b60fbc9aa714e55650ace47a05de81069`  
		Last Modified: Fri, 23 Apr 2021 23:54:57 GMT  
		Size: 14.1 MB (14087190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756fea3647fb5e2b8750dbb5e4c2fcf03f89f52b7e5cb55b7606924b2389ca81`  
		Last Modified: Fri, 23 Apr 2021 23:54:54 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fa9033e59f89cbb013c7d832613bab3a656300357cc70b7eade006a8edefce`  
		Last Modified: Fri, 23 Apr 2021 23:54:54 GMT  
		Size: 9.6 KB (9554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f62d4b9f7c9f91f8d9c689ebf626986dd4c2efd6d86ff851bd15bc6183dded0`  
		Last Modified: Fri, 23 Apr 2021 23:54:54 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491f6056574f25428a41b45fd180908c3bcb491ed462310db1dda218415df01c`  
		Last Modified: Fri, 23 Apr 2021 23:54:54 GMT  
		Size: 10.5 KB (10537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df697bb1f00968be2197f2465a5306f2873b7d22664eeb96b49f2a15ce43654d`  
		Last Modified: Fri, 23 Apr 2021 23:54:54 GMT  
		Size: 2.5 MB (2489469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.3-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:1f341387bf079c96efab0c7ab44b2c6043c03c9f996a0be98b076945c6bf10ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.3-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:3a4d36916ade30aabf91903a3a99226c23a9f07ff83d4507b8be5f06003da9dd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.1 MB (180147184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:559cc09d5d52e1c96eb02fda9d41efea67cd397625dd9cb0d5089aa21bf9ad6a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:30:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 09:31:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:31:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 09:31:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 09:31:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:31:17 GMT
ARG VERBOSE=false
# Fri, 26 Mar 2021 21:31:18 GMT
ARG OPENJ9_SCC=true
# Fri, 26 Mar 2021 21:31:18 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Fri, 26 Mar 2021 21:31:18 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Fri, 26 Mar 2021 21:31:18 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Fri, 26 Mar 2021 21:31:18 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 26 Mar 2021 21:31:19 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Fri, 26 Mar 2021 21:31:19 GMT
ARG LIBERTY_URL
# Fri, 26 Mar 2021 21:31:19 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 26 Mar 2021 21:31:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 21:31:33 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 21:31:33 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Fri, 26 Mar 2021 21:31:33 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 26 Mar 2021 21:31:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 26 Mar 2021 21:31:35 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 26 Mar 2021 21:31:35 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 26 Mar 2021 21:31:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 26 Mar 2021 21:31:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 26 Mar 2021 21:31:49 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:31:49 GMT
USER 1001
# Fri, 26 Mar 2021 21:31:49 GMT
EXPOSE 9080 9443
# Fri, 26 Mar 2021 21:31:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 26 Mar 2021 21:31:49 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4764ed71d2900c9874838108e377eb8821088502d5504fadeb080e5dd1a3e65d`  
		Last Modified: Fri, 26 Mar 2021 09:35:47 GMT  
		Size: 3.0 MB (2958415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf5000c541da177b7cfe59bf3ff8cb271529f443ee224bf88989910e9a2abb1`  
		Last Modified: Fri, 26 Mar 2021 09:36:01 GMT  
		Size: 130.8 MB (130805802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f62ff9f46b7fe8abf21ca3992ddfdba43c9a869ab05da497fd0c961b82bcc8`  
		Last Modified: Fri, 26 Mar 2021 21:49:10 GMT  
		Size: 14.0 MB (13988287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade44e6f5f910e4171dbe956b6f82444a1a0cf77cbb628a3cd3a4e02b91e4a75`  
		Last Modified: Fri, 26 Mar 2021 21:49:06 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e194224da53e4dca0cfb2e746e2dc2780faf558e27fbea8a051bbb1e645412a`  
		Last Modified: Fri, 26 Mar 2021 21:49:05 GMT  
		Size: 9.6 KB (9555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee645bef2bf69d54e107e8f571dd29a3a04a4bc4b3dc86db1e83a1cc15f0be9`  
		Last Modified: Fri, 26 Mar 2021 21:49:05 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7592107637fd3c10cd009e854a974a81b2a2bb14bbfc045924a369d59d3098`  
		Last Modified: Fri, 26 Mar 2021 21:49:05 GMT  
		Size: 10.5 KB (10545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11fedbbde6cf647ecb2604ada8a232f0040986bc0bab990ba49c28482ddc35f4`  
		Last Modified: Fri, 26 Mar 2021 21:49:07 GMT  
		Size: 5.7 MB (5661783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.3-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:92820e4f6e581eed9eb48670664b497a5f1213e8faefc06b49ab64c95dd138fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.2 MB (183163750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2091a3b41ecc0d00bc5021823c56cc35f4c9baaded519cd6f47a8aa72d57078`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:57:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 14:58:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:58:33 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 14:59:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 14:59:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:07:09 GMT
ARG VERBOSE=false
# Sat, 27 Mar 2021 05:07:11 GMT
ARG OPENJ9_SCC=true
# Sat, 27 Mar 2021 05:07:14 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Sat, 27 Mar 2021 05:07:16 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Sat, 27 Mar 2021 05:07:19 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Sat, 27 Mar 2021 05:07:23 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 27 Mar 2021 05:07:25 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Sat, 27 Mar 2021 05:07:28 GMT
ARG LIBERTY_URL
# Sat, 27 Mar 2021 05:07:30 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 27 Mar 2021 05:08:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:08:06 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 27 Mar 2021 05:08:09 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Sat, 27 Mar 2021 05:08:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 27 Mar 2021 05:08:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 27 Mar 2021 05:08:32 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Sat, 27 Mar 2021 05:08:34 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 27 Mar 2021 05:08:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 27 Mar 2021 05:09:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 27 Mar 2021 05:09:27 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:09:35 GMT
USER 1001
# Sat, 27 Mar 2021 05:09:41 GMT
EXPOSE 9080 9443
# Sat, 27 Mar 2021 05:09:44 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 27 Mar 2021 05:09:48 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a8b760dceb1369716f09f0677ac6e4c109c24e134a9c883c7e48e1ee0d081`  
		Last Modified: Fri, 26 Mar 2021 15:03:04 GMT  
		Size: 3.1 MB (3082734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c129b1161496dd5f093240bbcc3a8117babb3970d1b268b5ef2a3b583cf288`  
		Last Modified: Fri, 26 Mar 2021 15:03:19 GMT  
		Size: 130.4 MB (130406650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c71325e2d5617b9cd85e190ffdf8af663eb9617a1b6eccb340ab9de410d8e8`  
		Last Modified: Sat, 27 Mar 2021 05:38:58 GMT  
		Size: 14.0 MB (13989148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7124e4edcf5e13bc86bb8c43e5f200bd4a5f4510b57eba64f6f7451d46bd03`  
		Last Modified: Sat, 27 Mar 2021 05:38:51 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2088cb3daf47bf90822cb9bc806e51e7ce37ed6cc0c30909bff2fc88385d983b`  
		Last Modified: Sat, 27 Mar 2021 05:38:51 GMT  
		Size: 9.6 KB (9560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf52d46b34ad387623eef0aada894b720e268856356ec1c782d07b5b8f36561b`  
		Last Modified: Sat, 27 Mar 2021 05:38:52 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f72748eb637591c7ed93f76eca5bef63ff2233917f14fe3109f1b46e3a4e3b4`  
		Last Modified: Sat, 27 Mar 2021 05:38:51 GMT  
		Size: 10.5 KB (10535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0006e35e36fce96b51591922551d02cdfe5d95260d86017619492d5e429bbc62`  
		Last Modified: Sat, 27 Mar 2021 05:38:53 GMT  
		Size: 5.2 MB (5239852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.3-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:7ec7cd651e1f55c59b2ced91a2002ec8589bad439419f68c395622a287dad243
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.0 MB (175955005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74bec04b1307de7153f1bd7a3a2cf3022ed3d3f35064bd24ba6e28c45a27b5d1`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:25:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 23 Apr 2021 22:25:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:25:17 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 23 Apr 2021 22:26:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 23 Apr 2021 22:26:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:16:58 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:16:58 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:29:48 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Fri, 23 Apr 2021 23:29:49 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Fri, 23 Apr 2021 23:29:50 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Fri, 23 Apr 2021 23:29:50 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:29:51 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Fri, 23 Apr 2021 23:29:52 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:29:52 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:30:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:30:10 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:30:11 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Fri, 23 Apr 2021 23:30:11 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:30:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:30:15 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:30:15 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:30:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:30:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:30:32 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:30:33 GMT
USER 1001
# Fri, 23 Apr 2021 23:30:33 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:30:34 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:30:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93b87da546ac7aa6705cd2f20bfe70cf04793ac73561e5dd8c579af88754aec`  
		Last Modified: Fri, 23 Apr 2021 22:28:41 GMT  
		Size: 2.7 MB (2676643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268462fc02d2bd9da227784f5f243759923a14cefb3648739ca02e8fa7d63ee7`  
		Last Modified: Fri, 23 Apr 2021 22:28:50 GMT  
		Size: 128.1 MB (128065984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2e27878ce60350be68bbdb3b8ee9cbfde9b111787d0b974a06b8dffadddcbd`  
		Last Modified: Fri, 23 Apr 2021 23:54:49 GMT  
		Size: 14.0 MB (13988524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894cb19fa986a022ad70870257b92d2c0c4fb51aabb232cd0284dacada85fe2`  
		Last Modified: Fri, 23 Apr 2021 23:54:46 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08d76891a169b900915649827dc512feb56f753883fe52981be6f04d736b2f6`  
		Last Modified: Fri, 23 Apr 2021 23:54:46 GMT  
		Size: 9.6 KB (9557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34ee5d8f9435c0ed35bd9d1b5ae402ce58f34113d03dd5a315a826c6cd83b36`  
		Last Modified: Fri, 23 Apr 2021 23:54:46 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300d3fb2439110af45d80a2ddbf132b397feb71fefce3d1f0a596b771fdb90c`  
		Last Modified: Fri, 23 Apr 2021 23:54:47 GMT  
		Size: 10.5 KB (10543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a38e178e857d2811edcaca15881bfc7721e5afa49da3e0557037dfec12a23f`  
		Last Modified: Fri, 23 Apr 2021 23:54:47 GMT  
		Size: 5.8 MB (5848991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.4-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:8ae8aa183b83bb2caf4e9508d9049825f2b3067e4a713de5f3e21b89187911e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.4-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:35cc2096f3510a3db928f854c16a9bedad246d1252f311c839f1c572d9c73dff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.6 MB (329563878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a13fac28833e00b5e3a59ae871ccdd0fbdf78ae2ea63171016753dc05b77a32`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 01:29:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 01:29:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:32:52 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:10 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 21:40:48 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:40:48 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:48 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 21:40:49 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 21:40:49 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 21:40:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:40:49 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 21:40:49 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:40:49 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:40:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:40:58 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:40:58 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 21:40:58 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:41:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:41:00 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:41:00 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:41:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:41:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:41:09 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 22 Apr 2021 21:41:09 GMT
USER 1001
# Thu, 22 Apr 2021 21:41:10 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:41:10 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:41:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 21:44:55 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:44:55 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 21:47:40 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 21:47:41 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 21:48:15 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04b772c31f76720583412a2507c5c53889985db45169a85f0d3cd7f842e041a`  
		Last Modified: Sat, 03 Apr 2021 01:39:30 GMT  
		Size: 16.0 MB (16032891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf71362343a962febc8c6ce8c4fd12d961c5712407993471f60ac0e5d43415e`  
		Last Modified: Mon, 19 Apr 2021 18:30:17 GMT  
		Size: 42.4 MB (42440313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9163852ff25e45c3b95c7b759a719b91afa29724136e68d1cf7f822c034c4df`  
		Last Modified: Mon, 19 Apr 2021 18:30:04 GMT  
		Size: 4.0 MB (4025359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a723eb5427857d3e6f939a462cbbaeedb1b248662076fe72f2fab621d9acc3`  
		Last Modified: Thu, 22 Apr 2021 21:57:15 GMT  
		Size: 14.2 MB (14160245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0598dd9101a4447350e39fc9445131bdeb5a9bee7fc233879f0451c08a79fe`  
		Last Modified: Thu, 22 Apr 2021 21:57:12 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf163d48e000642c258afeea2bb09c0cca8829f72fcd792c97840c181f7331f8`  
		Last Modified: Thu, 22 Apr 2021 21:57:12 GMT  
		Size: 9.6 KB (9550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5906189dfc1fa00888b59c4cefad5a2f4aa3085bcc6da5d37e63197585a231c`  
		Last Modified: Thu, 22 Apr 2021 21:57:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062608db9cb7d8e8fc2dfa23464525e84b5d5fe1bc979194b937d8b2a4de74a6`  
		Last Modified: Thu, 22 Apr 2021 21:57:11 GMT  
		Size: 10.5 KB (10531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2d74ce76564c5e8a6dafde72882602b446b3d3d81d620c5b1f08232a5a019`  
		Last Modified: Thu, 22 Apr 2021 21:57:11 GMT  
		Size: 2.6 MB (2555007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2717086accd7d50a5527b2b70f1177f08e904718f5388f702983ce093761304`  
		Last Modified: Thu, 22 Apr 2021 21:58:02 GMT  
		Size: 207.7 MB (207669936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59e20e338e249cff7c3435973456929f13dfea41138604d3fe1696e479dc61`  
		Last Modified: Thu, 22 Apr 2021 21:57:50 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455eb33d7a0b34ae7cec9f9f41505c10dd6db2bd14f0f792b193a312a1c64b9e`  
		Last Modified: Thu, 22 Apr 2021 21:57:53 GMT  
		Size: 14.1 MB (14088088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.4-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:07540a882ea5483563b694c0dad8ae082abd9ae8c39c96be69a8730b843f0804
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.5 MB (334547474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c92dca05464955a0c79c7e5f82f7489fc4727cf3a74c5cea077620bb7a4fd42f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 05:41:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 05:43:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 05:51:38 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:15 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 22:40:19 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:40:26 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:40:30 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 22:40:33 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 22:40:37 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 22:40:40 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 22:40:45 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 22:40:52 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 22:40:56 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 22:41:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 22:41:46 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 22:41:56 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 22:42:04 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:42:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 22:42:23 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 22:42:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 22:42:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 22:43:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 22:43:11 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 22 Apr 2021 22:43:15 GMT
USER 1001
# Thu, 22 Apr 2021 22:43:19 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 22:43:24 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 22:43:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 22:49:54 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:49:59 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 22:53:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 22:54:02 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 22:55:14 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3147f9d7021e4b4f874d531cd0d820bd489543f00c894d4d9df8f2c1b0777d2b`  
		Last Modified: Sat, 03 Apr 2021 06:01:07 GMT  
		Size: 17.2 MB (17208203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422c588ac4abf48f1a915be1f8f943b1dbc48565bc9f3816ef2bc82f6eb2b9e9`  
		Last Modified: Mon, 19 Apr 2021 18:33:46 GMT  
		Size: 43.3 MB (43277555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e121c025bd5ea767e5c45ee767dc2033229a9d9fb8d83a441bd012a380fd`  
		Last Modified: Mon, 19 Apr 2021 18:33:34 GMT  
		Size: 3.3 MB (3280395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6929ab0e248a58c5b49948573b1127df1bcbe68796a5e21814a4c9e4e28f6ebf`  
		Last Modified: Thu, 22 Apr 2021 23:13:18 GMT  
		Size: 14.2 MB (14161071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2588e073d28ae56c3b8dfd39e5a1d6dccae837dd371077e43397444ffb8ff1e`  
		Last Modified: Thu, 22 Apr 2021 23:13:11 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a98cf9a7933225976737f1a20308355729c508995402133840fcc479f27d43`  
		Last Modified: Thu, 22 Apr 2021 23:13:12 GMT  
		Size: 9.6 KB (9551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac8f8e29ad8d0df0b59f8076e79f3af0ff5d168e821f3cd7ac29b1d58ab08f1`  
		Last Modified: Thu, 22 Apr 2021 23:13:11 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1f252245d30a42990c0c73190e7139531fa283f5d7ee5ebd4df55dfe374412`  
		Last Modified: Thu, 22 Apr 2021 23:13:11 GMT  
		Size: 10.5 KB (10543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef9dd9d762820f249356fcd609a933f771ea6d3958711f43e56650e6507342c`  
		Last Modified: Thu, 22 Apr 2021 23:13:12 GMT  
		Size: 2.5 MB (2452650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8319ed53797eb366322fe8e99f98580a1331d4816d5144074d9cadca6cd789c`  
		Last Modified: Thu, 22 Apr 2021 23:14:21 GMT  
		Size: 207.7 MB (207671859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf42350fcce58dfd0beca958548225d94e2ffb95de42637e27781977f3842d2`  
		Last Modified: Thu, 22 Apr 2021 23:14:00 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d061bc3e9092696be441f9b782f5d6cbfaf1b296a48f5c8469817146c5386`  
		Last Modified: Thu, 22 Apr 2021 23:14:03 GMT  
		Size: 13.2 MB (13192654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.4-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0d02e361435df46fff35ebc173579ebb1dafbc0713fa6fa5882156f0ac9abb76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.6 MB (326645376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c382f67d2996379923080d0c01ae3039c6ef3b9f1e0b452d32958d81cd7e7487`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:03:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 22:04:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:10:11 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Fri, 23 Apr 2021 22:11:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 23 Apr 2021 22:11:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 22:11:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 23 Apr 2021 22:12:20 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 23 Apr 2021 23:17:55 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:17:56 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:17:56 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Fri, 23 Apr 2021 23:17:57 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Fri, 23 Apr 2021 23:17:57 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Fri, 23 Apr 2021 23:17:58 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:17:59 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Fri, 23 Apr 2021 23:17:59 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:18:00 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:18:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:18:15 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:18:16 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Fri, 23 Apr 2021 23:18:16 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:18:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:18:19 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:18:19 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:18:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:18:32 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:18:33 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Fri, 23 Apr 2021 23:18:34 GMT
USER 1001
# Fri, 23 Apr 2021 23:18:35 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:18:36 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:18:36 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 23 Apr 2021 23:24:07 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:24:07 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 23 Apr 2021 23:28:09 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 23 Apr 2021 23:28:21 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 23 Apr 2021 23:29:08 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bab416938acf6dd045c9fc9097e5768c61b5899b07d110ab3844f447e12b113`  
		Last Modified: Fri, 23 Apr 2021 22:19:05 GMT  
		Size: 15.7 MB (15741779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0273d3bc7cd55960a36b00d19e8d51f8bbeed03d24fd8d551c957fc19ef079b`  
		Last Modified: Fri, 23 Apr 2021 22:22:19 GMT  
		Size: 42.0 MB (41951613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95422aa686364d2877a279281f6eb1157805fa8516aa976b06ce8889dc9f932`  
		Last Modified: Fri, 23 Apr 2021 22:22:13 GMT  
		Size: 3.8 MB (3836026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f024126ee5e04e37dd48573fe2e6aefd2d98012df116b366e0aef9fa63b8ba93`  
		Last Modified: Fri, 23 Apr 2021 23:54:00 GMT  
		Size: 14.2 MB (14160729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a63a9d57fd3b2ed838f0044559d5cfa241eab25d7626378b2fd1c5463947a9`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 687.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62def58659c4a5a6fd3cde1c4245691f62a7d197ac87536975c7c888e8fd5ff`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 9.6 KB (9551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288fec31697eb659f1a7285ca37ce8460c07bd8485fdb21628ff246a6661660d`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bce08718a41817d4e1e9dd6bb83ac83f3a1c3014753a04447805c257e51a9c3`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 10.5 KB (10544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3096c60acccc8db5e2ef0df733a4693cf8068658a1fc8af639461c112c1589a`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 2.5 MB (2491647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d29297ab00722488619fd9526e89b49277ed66bac34206e8f7e2cb0917e1945`  
		Last Modified: Fri, 23 Apr 2021 23:54:35 GMT  
		Size: 207.7 MB (207671747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b7a66a256bd33f418c1622886d5384d5a5abc02e2c3b042d528a7153211728`  
		Last Modified: Fri, 23 Apr 2021 23:54:24 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba111cf88078cf3a5f862c69d813cf4940c21337daefa46d9c6a9818aae58d8e`  
		Last Modified: Fri, 23 Apr 2021 23:54:26 GMT  
		Size: 13.6 MB (13632445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.4-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:094c65417cc16f118454ebe6006581e60ef033253453edcf99997082200bcd87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.4-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:750da2549ddcfbd3e9ae2850b9ae2347adbb712410041faf8a02a81d635d2cde
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.8 MB (414810589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bfd08f9c2afdc6e2530607e9db350908221943ae7b3a387ed47fde3bad081c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:30:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 09:31:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:31:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 09:31:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 09:31:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:31:17 GMT
ARG VERBOSE=false
# Fri, 26 Mar 2021 21:31:18 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:06 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 21:40:06 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 21:40:06 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 21:40:06 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:40:06 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 21:40:07 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:40:07 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:40:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:40:24 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:40:24 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 21:40:24 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:40:26 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:40:26 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:40:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:40:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:40:38 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 22 Apr 2021 21:40:38 GMT
USER 1001
# Thu, 22 Apr 2021 21:40:39 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:40:39 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:40:39 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 21:41:13 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:41:13 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 21:44:16 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 21:44:16 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 21:44:52 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4764ed71d2900c9874838108e377eb8821088502d5504fadeb080e5dd1a3e65d`  
		Last Modified: Fri, 26 Mar 2021 09:35:47 GMT  
		Size: 3.0 MB (2958415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf5000c541da177b7cfe59bf3ff8cb271529f443ee224bf88989910e9a2abb1`  
		Last Modified: Fri, 26 Mar 2021 09:36:01 GMT  
		Size: 130.8 MB (130805802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df46370333075337eb25c08aa74c706467351aa5abe9711e870aa5e647baaf`  
		Last Modified: Thu, 22 Apr 2021 21:57:02 GMT  
		Size: 14.1 MB (14061162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d854faca6db468012fcae8e445cd69affeb82c5efbb89ac2b53b719cb4eabd`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f56d571437c689e2188bb2653cbbaf3ef56de28093fd63e3229a142d9d87fa`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 9.6 KB (9556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fde75a052b81ad9ca202510ebedb5083754ed163d499a6f28f1be76b6615ad`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610a90e750f1b7eb794e24a2970acb3b9f79a569ed064d70771895e2cf5c4795`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 10.5 KB (10544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3782c27b14b1eea6ec7f8a3c56182ccbf3a0db0e5a00cb4aad829f8b16f628b1`  
		Last Modified: Thu, 22 Apr 2021 21:56:59 GMT  
		Size: 5.7 MB (5734998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f94a4feba9d432ba504a626d7c726342855fc5baffbda070b24e905aa4d6f2`  
		Last Modified: Thu, 22 Apr 2021 21:57:36 GMT  
		Size: 213.4 MB (213364505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f32f1e0b41195d19cb5b1bc063af6b2ebd037fee723a18c58cee092d68b465`  
		Last Modified: Thu, 22 Apr 2021 21:57:24 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926bbbd582bf41deb09392c6714bc00b03c3a35a16db042c445f171588d03f52`  
		Last Modified: Thu, 22 Apr 2021 21:57:28 GMT  
		Size: 21.2 MB (21151866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.4-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:faecb180eab0cf2e7ef66b023b667894577ba036211d2ecfe90253d136799327
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.0 MB (415020984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2632640bf1740b9f968ae52aa680b98fa04477aab0660c8baf5b8fddf79bf0a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:57:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 14:58:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:58:33 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 14:59:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 14:59:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:07:09 GMT
ARG VERBOSE=false
# Sat, 27 Mar 2021 05:07:11 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:36:22 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 22:36:27 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 22:36:31 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 22:36:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 22:36:37 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 22:36:41 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 22:36:46 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 22:38:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 22:38:05 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 22:38:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 22:38:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:38:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 22:38:41 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 22:38:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 22:39:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 22:39:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 22:39:38 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 22 Apr 2021 22:39:41 GMT
USER 1001
# Thu, 22 Apr 2021 22:39:45 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 22:39:51 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 22:39:55 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 22:43:49 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:43:55 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 22:48:08 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 22:48:12 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 22:49:35 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a8b760dceb1369716f09f0677ac6e4c109c24e134a9c883c7e48e1ee0d081`  
		Last Modified: Fri, 26 Mar 2021 15:03:04 GMT  
		Size: 3.1 MB (3082734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c129b1161496dd5f093240bbcc3a8117babb3970d1b268b5ef2a3b583cf288`  
		Last Modified: Fri, 26 Mar 2021 15:03:19 GMT  
		Size: 130.4 MB (130406650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec06bab51d83666979940922b947a720f6acaca816d2bf3cd332e567591afa4b`  
		Last Modified: Thu, 22 Apr 2021 23:13:03 GMT  
		Size: 14.1 MB (14062057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7f4311425eb37ef28297f5763e749844d439a78264d4863390508759094d6`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1685eb89d16b4bfbe9ff198cfccf641c1de3b8ea23ef56df88b431fed4260572`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 9.6 KB (9557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2045df8ec68a9c233ea9c9dcb3fb5568ea59166bb9912373e550945f7c42c1f`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc56667d904c50234135b3bfefa6630c14e255a6fbd7ee3143d06f8aac839ab9`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 10.6 KB (10553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5451ef86b75da4eaad3a9248b4b2158b6aca3cb0a19da6c9dfc7a955e8de2038`  
		Last Modified: Thu, 22 Apr 2021 23:12:59 GMT  
		Size: 5.3 MB (5327202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbb2811058d1ddf7c93605f52b4f92cf27c033ae5b026fb74b7584705122c15`  
		Last Modified: Thu, 22 Apr 2021 23:13:48 GMT  
		Size: 213.0 MB (212960397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab321d9643cb04efbdeaff3e7e94f91bd291323f304fc7b2943c5578468939e`  
		Last Modified: Thu, 22 Apr 2021 23:13:26 GMT  
		Size: 953.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edfcc0e4989bb4f0adce15dd3e622084b8b2c6ea9f85223785b1f7bcd097a5d`  
		Last Modified: Thu, 22 Apr 2021 23:13:31 GMT  
		Size: 18.7 MB (18735600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.4-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:1813d2e44e1f79784ab44778359fd80a47b37726d4ded32db082ca08eb72f80f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.0 MB (411023034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1109636c471215912302d8affaad06caa663cedee902a569c14ebc0e70e6a9a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:25:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 23 Apr 2021 22:25:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:25:17 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 23 Apr 2021 22:26:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 23 Apr 2021 22:26:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:16:58 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:16:58 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:16:59 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Fri, 23 Apr 2021 23:17:00 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Fri, 23 Apr 2021 23:17:00 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Fri, 23 Apr 2021 23:17:01 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:17:02 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Fri, 23 Apr 2021 23:17:02 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:17:03 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:17:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:17:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:17:21 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Fri, 23 Apr 2021 23:17:21 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:17:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:17:24 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:17:25 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:17:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:17:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:17:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:17:42 GMT
USER 1001
# Fri, 23 Apr 2021 23:17:42 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:17:43 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:17:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 23 Apr 2021 23:18:44 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:18:45 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 23 Apr 2021 23:22:46 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 23 Apr 2021 23:23:00 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 23 Apr 2021 23:23:44 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93b87da546ac7aa6705cd2f20bfe70cf04793ac73561e5dd8c579af88754aec`  
		Last Modified: Fri, 23 Apr 2021 22:28:41 GMT  
		Size: 2.7 MB (2676643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268462fc02d2bd9da227784f5f243759923a14cefb3648739ca02e8fa7d63ee7`  
		Last Modified: Fri, 23 Apr 2021 22:28:50 GMT  
		Size: 128.1 MB (128065984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895091e75a5c1ee863c074a41c334973d986bb55cef3d4ba2f8267a2887f8336`  
		Last Modified: Fri, 23 Apr 2021 23:53:50 GMT  
		Size: 14.1 MB (14061390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26d2145efe41abadeb2694f43164f1a155e500e85bf004da26812cd8532de7f`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1dc41aa938b0af86dfd6446147e4484cb5d6bad6e84eb2edb074790b0615a1`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 9.6 KB (9556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0e2666f7e25fefd1dfbbb522189283388626a78a6993958a175bfe3d453daa`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1422da1f78c4ff3f196f908ccd43d884e84e4586193eab1bfe59df39b352b130`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 10.5 KB (10540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a848b971c7539a51ff9771c57f7df448cc5b960c0be0fa5b3c3b547e8589c`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 5.9 MB (5924580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a29d9ef14335af914d1a4155de231f338e3649b1e962477e8f3c3007227195`  
		Last Modified: Fri, 23 Apr 2021 23:54:16 GMT  
		Size: 213.6 MB (213555213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85098d48d9a85bbbdc1b5f863692bf7b326b94c5f44d091ff39e53fb34a41cc`  
		Last Modified: Fri, 23 Apr 2021 23:54:05 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1e656c995305a66ce28c668c88b221183600d735978d891b72351644e890c2`  
		Last Modified: Fri, 23 Apr 2021 23:54:08 GMT  
		Size: 21.4 MB (21363413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.4-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:fe1abe1b8727e22b222d63ad4486ef6da1e3018131b94234fe5977ee4b59a8f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.4-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:089c25ea4ac42c4cedb0b974d8cf29185eb9c3ec4e86fa10817a8afa5de7f601
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107804910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98fb4f6747d498676b24bc7bf8aa4905b802d1f2ed2d3b27bce67a59d00748c5`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 01:29:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 01:29:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:32:52 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:10 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 21:40:48 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:40:48 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:48 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 21:40:49 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 21:40:49 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 21:40:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:40:49 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 21:40:49 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:40:49 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:40:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:40:58 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:40:58 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 21:40:58 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:41:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:41:00 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:41:00 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:41:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:41:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:41:09 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 22 Apr 2021 21:41:09 GMT
USER 1001
# Thu, 22 Apr 2021 21:41:10 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:41:10 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:41:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04b772c31f76720583412a2507c5c53889985db45169a85f0d3cd7f842e041a`  
		Last Modified: Sat, 03 Apr 2021 01:39:30 GMT  
		Size: 16.0 MB (16032891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf71362343a962febc8c6ce8c4fd12d961c5712407993471f60ac0e5d43415e`  
		Last Modified: Mon, 19 Apr 2021 18:30:17 GMT  
		Size: 42.4 MB (42440313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9163852ff25e45c3b95c7b759a719b91afa29724136e68d1cf7f822c034c4df`  
		Last Modified: Mon, 19 Apr 2021 18:30:04 GMT  
		Size: 4.0 MB (4025359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a723eb5427857d3e6f939a462cbbaeedb1b248662076fe72f2fab621d9acc3`  
		Last Modified: Thu, 22 Apr 2021 21:57:15 GMT  
		Size: 14.2 MB (14160245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0598dd9101a4447350e39fc9445131bdeb5a9bee7fc233879f0451c08a79fe`  
		Last Modified: Thu, 22 Apr 2021 21:57:12 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf163d48e000642c258afeea2bb09c0cca8829f72fcd792c97840c181f7331f8`  
		Last Modified: Thu, 22 Apr 2021 21:57:12 GMT  
		Size: 9.6 KB (9550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5906189dfc1fa00888b59c4cefad5a2f4aa3085bcc6da5d37e63197585a231c`  
		Last Modified: Thu, 22 Apr 2021 21:57:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062608db9cb7d8e8fc2dfa23464525e84b5d5fe1bc979194b937d8b2a4de74a6`  
		Last Modified: Thu, 22 Apr 2021 21:57:11 GMT  
		Size: 10.5 KB (10531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2d74ce76564c5e8a6dafde72882602b446b3d3d81d620c5b1f08232a5a019`  
		Last Modified: Thu, 22 Apr 2021 21:57:11 GMT  
		Size: 2.6 MB (2555007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.4-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:db1df505afa055570fd1730ad5546e03de17d85d4e49d3758b8f46f2d706a977
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113682013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77818b750cad7803852ce86ef76b32a4d32276ef03279d867bedee73e1663156`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 05:41:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 05:43:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 05:51:38 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:15 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 22:40:19 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:40:26 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:40:30 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 22:40:33 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 22:40:37 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 22:40:40 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 22:40:45 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 22:40:52 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 22:40:56 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 22:41:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 22:41:46 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 22:41:56 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 22:42:04 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:42:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 22:42:23 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 22:42:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 22:42:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 22:43:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 22:43:11 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 22 Apr 2021 22:43:15 GMT
USER 1001
# Thu, 22 Apr 2021 22:43:19 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 22:43:24 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 22:43:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3147f9d7021e4b4f874d531cd0d820bd489543f00c894d4d9df8f2c1b0777d2b`  
		Last Modified: Sat, 03 Apr 2021 06:01:07 GMT  
		Size: 17.2 MB (17208203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422c588ac4abf48f1a915be1f8f943b1dbc48565bc9f3816ef2bc82f6eb2b9e9`  
		Last Modified: Mon, 19 Apr 2021 18:33:46 GMT  
		Size: 43.3 MB (43277555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e121c025bd5ea767e5c45ee767dc2033229a9d9fb8d83a441bd012a380fd`  
		Last Modified: Mon, 19 Apr 2021 18:33:34 GMT  
		Size: 3.3 MB (3280395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6929ab0e248a58c5b49948573b1127df1bcbe68796a5e21814a4c9e4e28f6ebf`  
		Last Modified: Thu, 22 Apr 2021 23:13:18 GMT  
		Size: 14.2 MB (14161071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2588e073d28ae56c3b8dfd39e5a1d6dccae837dd371077e43397444ffb8ff1e`  
		Last Modified: Thu, 22 Apr 2021 23:13:11 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a98cf9a7933225976737f1a20308355729c508995402133840fcc479f27d43`  
		Last Modified: Thu, 22 Apr 2021 23:13:12 GMT  
		Size: 9.6 KB (9551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac8f8e29ad8d0df0b59f8076e79f3af0ff5d168e821f3cd7ac29b1d58ab08f1`  
		Last Modified: Thu, 22 Apr 2021 23:13:11 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1f252245d30a42990c0c73190e7139531fa283f5d7ee5ebd4df55dfe374412`  
		Last Modified: Thu, 22 Apr 2021 23:13:11 GMT  
		Size: 10.5 KB (10543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef9dd9d762820f249356fcd609a933f771ea6d3958711f43e56650e6507342c`  
		Last Modified: Thu, 22 Apr 2021 23:13:12 GMT  
		Size: 2.5 MB (2452650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.4-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:7da2d996a0edd7759eef333322be612a3aa048d1c48ffec09bef5d1d8aca195e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105340236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0450ad9b23e181ff9223541e51f3bd15bdc098a0b0e011fda20432f21f2b5467`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:03:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 22:04:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:10:11 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Fri, 23 Apr 2021 22:11:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 23 Apr 2021 22:11:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 22:11:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 23 Apr 2021 22:12:20 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 23 Apr 2021 23:17:55 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:17:56 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:17:56 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Fri, 23 Apr 2021 23:17:57 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Fri, 23 Apr 2021 23:17:57 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Fri, 23 Apr 2021 23:17:58 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:17:59 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Fri, 23 Apr 2021 23:17:59 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:18:00 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:18:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:18:15 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:18:16 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Fri, 23 Apr 2021 23:18:16 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:18:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:18:19 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:18:19 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:18:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:18:32 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:18:33 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Fri, 23 Apr 2021 23:18:34 GMT
USER 1001
# Fri, 23 Apr 2021 23:18:35 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:18:36 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:18:36 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bab416938acf6dd045c9fc9097e5768c61b5899b07d110ab3844f447e12b113`  
		Last Modified: Fri, 23 Apr 2021 22:19:05 GMT  
		Size: 15.7 MB (15741779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0273d3bc7cd55960a36b00d19e8d51f8bbeed03d24fd8d551c957fc19ef079b`  
		Last Modified: Fri, 23 Apr 2021 22:22:19 GMT  
		Size: 42.0 MB (41951613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95422aa686364d2877a279281f6eb1157805fa8516aa976b06ce8889dc9f932`  
		Last Modified: Fri, 23 Apr 2021 22:22:13 GMT  
		Size: 3.8 MB (3836026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f024126ee5e04e37dd48573fe2e6aefd2d98012df116b366e0aef9fa63b8ba93`  
		Last Modified: Fri, 23 Apr 2021 23:54:00 GMT  
		Size: 14.2 MB (14160729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a63a9d57fd3b2ed838f0044559d5cfa241eab25d7626378b2fd1c5463947a9`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 687.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62def58659c4a5a6fd3cde1c4245691f62a7d197ac87536975c7c888e8fd5ff`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 9.6 KB (9551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288fec31697eb659f1a7285ca37ce8460c07bd8485fdb21628ff246a6661660d`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bce08718a41817d4e1e9dd6bb83ac83f3a1c3014753a04447805c257e51a9c3`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 10.5 KB (10544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3096c60acccc8db5e2ef0df733a4693cf8068658a1fc8af639461c112c1589a`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 2.5 MB (2491647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.4-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:8eb580730060d28e69050bde292ec263ccd5d9dfc7f50947d700aef92cadd471
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.4-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:f528365190e853e1ffbc72c586114358fb2eb6e0117c4134f68e0e57894f6f24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180293270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79615f972bc823a2954599784f3311d9cd8c7d4e5bc2ee82a917c4f753326937`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:30:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 09:31:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:31:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 09:31:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 09:31:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:31:17 GMT
ARG VERBOSE=false
# Fri, 26 Mar 2021 21:31:18 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:06 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 21:40:06 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 21:40:06 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 21:40:06 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:40:06 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 21:40:07 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:40:07 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:40:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:40:24 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:40:24 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 21:40:24 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:40:26 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:40:26 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:40:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:40:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:40:38 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 22 Apr 2021 21:40:38 GMT
USER 1001
# Thu, 22 Apr 2021 21:40:39 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:40:39 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:40:39 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4764ed71d2900c9874838108e377eb8821088502d5504fadeb080e5dd1a3e65d`  
		Last Modified: Fri, 26 Mar 2021 09:35:47 GMT  
		Size: 3.0 MB (2958415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf5000c541da177b7cfe59bf3ff8cb271529f443ee224bf88989910e9a2abb1`  
		Last Modified: Fri, 26 Mar 2021 09:36:01 GMT  
		Size: 130.8 MB (130805802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df46370333075337eb25c08aa74c706467351aa5abe9711e870aa5e647baaf`  
		Last Modified: Thu, 22 Apr 2021 21:57:02 GMT  
		Size: 14.1 MB (14061162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d854faca6db468012fcae8e445cd69affeb82c5efbb89ac2b53b719cb4eabd`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f56d571437c689e2188bb2653cbbaf3ef56de28093fd63e3229a142d9d87fa`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 9.6 KB (9556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fde75a052b81ad9ca202510ebedb5083754ed163d499a6f28f1be76b6615ad`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610a90e750f1b7eb794e24a2970acb3b9f79a569ed064d70771895e2cf5c4795`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 10.5 KB (10544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3782c27b14b1eea6ec7f8a3c56182ccbf3a0db0e5a00cb4aad829f8b16f628b1`  
		Last Modified: Thu, 22 Apr 2021 21:56:59 GMT  
		Size: 5.7 MB (5734998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.4-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:6322cd5c750764e7efee92c0f43a9cdffade75d0c8480ab4c7c24ed8c5b3af2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.3 MB (183324034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc735b0a89ae88f071398c01160e7248b957a412c35d93bb33bfbc5575693f9c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:57:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 14:58:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:58:33 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 14:59:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 14:59:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:07:09 GMT
ARG VERBOSE=false
# Sat, 27 Mar 2021 05:07:11 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:36:22 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 22:36:27 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 22:36:31 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 22:36:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 22:36:37 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 22:36:41 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 22:36:46 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 22:38:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 22:38:05 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 22:38:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 22:38:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:38:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 22:38:41 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 22:38:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 22:39:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 22:39:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 22:39:38 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 22 Apr 2021 22:39:41 GMT
USER 1001
# Thu, 22 Apr 2021 22:39:45 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 22:39:51 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 22:39:55 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a8b760dceb1369716f09f0677ac6e4c109c24e134a9c883c7e48e1ee0d081`  
		Last Modified: Fri, 26 Mar 2021 15:03:04 GMT  
		Size: 3.1 MB (3082734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c129b1161496dd5f093240bbcc3a8117babb3970d1b268b5ef2a3b583cf288`  
		Last Modified: Fri, 26 Mar 2021 15:03:19 GMT  
		Size: 130.4 MB (130406650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec06bab51d83666979940922b947a720f6acaca816d2bf3cd332e567591afa4b`  
		Last Modified: Thu, 22 Apr 2021 23:13:03 GMT  
		Size: 14.1 MB (14062057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7f4311425eb37ef28297f5763e749844d439a78264d4863390508759094d6`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1685eb89d16b4bfbe9ff198cfccf641c1de3b8ea23ef56df88b431fed4260572`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 9.6 KB (9557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2045df8ec68a9c233ea9c9dcb3fb5568ea59166bb9912373e550945f7c42c1f`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc56667d904c50234135b3bfefa6630c14e255a6fbd7ee3143d06f8aac839ab9`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 10.6 KB (10553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5451ef86b75da4eaad3a9248b4b2158b6aca3cb0a19da6c9dfc7a955e8de2038`  
		Last Modified: Thu, 22 Apr 2021 23:12:59 GMT  
		Size: 5.3 MB (5327202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.4-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0d7dafd042d0d2cc8eb4580d0db30ada5047e8848c332172235044b128158d2f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176103462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a099f0ae43c0fd8c3e964020f65971f96b5f6988450d42231f7333bb9b4fb8f2`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:25:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 23 Apr 2021 22:25:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:25:17 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 23 Apr 2021 22:26:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 23 Apr 2021 22:26:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:16:58 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:16:58 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:16:59 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Fri, 23 Apr 2021 23:17:00 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Fri, 23 Apr 2021 23:17:00 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Fri, 23 Apr 2021 23:17:01 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:17:02 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Fri, 23 Apr 2021 23:17:02 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:17:03 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:17:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:17:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:17:21 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Fri, 23 Apr 2021 23:17:21 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:17:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:17:24 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:17:25 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:17:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:17:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:17:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:17:42 GMT
USER 1001
# Fri, 23 Apr 2021 23:17:42 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:17:43 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:17:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93b87da546ac7aa6705cd2f20bfe70cf04793ac73561e5dd8c579af88754aec`  
		Last Modified: Fri, 23 Apr 2021 22:28:41 GMT  
		Size: 2.7 MB (2676643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268462fc02d2bd9da227784f5f243759923a14cefb3648739ca02e8fa7d63ee7`  
		Last Modified: Fri, 23 Apr 2021 22:28:50 GMT  
		Size: 128.1 MB (128065984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895091e75a5c1ee863c074a41c334973d986bb55cef3d4ba2f8267a2887f8336`  
		Last Modified: Fri, 23 Apr 2021 23:53:50 GMT  
		Size: 14.1 MB (14061390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26d2145efe41abadeb2694f43164f1a155e500e85bf004da26812cd8532de7f`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1dc41aa938b0af86dfd6446147e4484cb5d6bad6e84eb2edb074790b0615a1`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 9.6 KB (9556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0e2666f7e25fefd1dfbbb522189283388626a78a6993958a175bfe3d453daa`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1422da1f78c4ff3f196f908ccd43d884e84e4586193eab1bfe59df39b352b130`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 10.5 KB (10540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a848b971c7539a51ff9771c57f7df448cc5b960c0be0fa5b3c3b547e8589c`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 5.9 MB (5924580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full`

```console
$ docker pull websphere-liberty@sha256:c57170761ec676e97a6a99f5004cc3080789d3b9f985247ff8cc1ecd50ff5c1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:750da2549ddcfbd3e9ae2850b9ae2347adbb712410041faf8a02a81d635d2cde
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.8 MB (414810589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bfd08f9c2afdc6e2530607e9db350908221943ae7b3a387ed47fde3bad081c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:30:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 09:31:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:31:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 09:31:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 09:31:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:31:17 GMT
ARG VERBOSE=false
# Fri, 26 Mar 2021 21:31:18 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:06 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 21:40:06 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 21:40:06 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 21:40:06 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:40:06 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 21:40:07 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:40:07 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:40:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:40:24 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:40:24 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 21:40:24 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:40:26 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:40:26 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:40:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:40:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:40:38 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 22 Apr 2021 21:40:38 GMT
USER 1001
# Thu, 22 Apr 2021 21:40:39 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:40:39 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:40:39 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 21:41:13 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:41:13 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 21:44:16 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 21:44:16 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 21:44:52 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4764ed71d2900c9874838108e377eb8821088502d5504fadeb080e5dd1a3e65d`  
		Last Modified: Fri, 26 Mar 2021 09:35:47 GMT  
		Size: 3.0 MB (2958415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf5000c541da177b7cfe59bf3ff8cb271529f443ee224bf88989910e9a2abb1`  
		Last Modified: Fri, 26 Mar 2021 09:36:01 GMT  
		Size: 130.8 MB (130805802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df46370333075337eb25c08aa74c706467351aa5abe9711e870aa5e647baaf`  
		Last Modified: Thu, 22 Apr 2021 21:57:02 GMT  
		Size: 14.1 MB (14061162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d854faca6db468012fcae8e445cd69affeb82c5efbb89ac2b53b719cb4eabd`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f56d571437c689e2188bb2653cbbaf3ef56de28093fd63e3229a142d9d87fa`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 9.6 KB (9556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fde75a052b81ad9ca202510ebedb5083754ed163d499a6f28f1be76b6615ad`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610a90e750f1b7eb794e24a2970acb3b9f79a569ed064d70771895e2cf5c4795`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 10.5 KB (10544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3782c27b14b1eea6ec7f8a3c56182ccbf3a0db0e5a00cb4aad829f8b16f628b1`  
		Last Modified: Thu, 22 Apr 2021 21:56:59 GMT  
		Size: 5.7 MB (5734998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f94a4feba9d432ba504a626d7c726342855fc5baffbda070b24e905aa4d6f2`  
		Last Modified: Thu, 22 Apr 2021 21:57:36 GMT  
		Size: 213.4 MB (213364505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f32f1e0b41195d19cb5b1bc063af6b2ebd037fee723a18c58cee092d68b465`  
		Last Modified: Thu, 22 Apr 2021 21:57:24 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926bbbd582bf41deb09392c6714bc00b03c3a35a16db042c445f171588d03f52`  
		Last Modified: Thu, 22 Apr 2021 21:57:28 GMT  
		Size: 21.2 MB (21151866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; 386

```console
$ docker pull websphere-liberty@sha256:c847143995aec30ca5d4526544d7c41ca7a42a8baf8195848864d0128e96ecf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.2 MB (349209019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d2c9374be56a63d6e35820fec8676f2d4ed2b9bdaf09a49c8545b039479bb7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:38:55 GMT
ADD file:d859d389e38b7ac70fd56f97e38d52a77b58e72b96237a4302d1984cdd912a55 in / 
# Fri, 20 Mar 2020 18:38:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:38:57 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:38:58 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:38:58 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:06:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 20 Mar 2020 19:06:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:06:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp6
# Fri, 20 Mar 2020 19:07:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='87f9d45b7e1fa65ec018479f3ca7da69a03b52b0da10b8d1555142eec8ab0093';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='b5f825047c9bb5d360fb83694f12e17b1a5a15abf94ac82cd0a3aea32c9a361c';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f3c04cd07ef269c24373840eae6f59c7db7a16d2e206d393ba93efa6dbb8d74f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2bbefda96f7d1a5f1694893961e92ccc59dfa50375ae5450675d7a4213d5812e';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='d5b0508d53d1c7382c06f5bc1daf3d57c19c70d851e86e6b1162bcd93f616f7e';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 20 Mar 2020 19:07:26 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:31:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433
# Fri, 20 Mar 2020 19:31:53 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Fri, 20 Mar 2020 19:31:53 GMT
ARG LIBERTY_URL
# Fri, 20 Mar 2020 19:31:53 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 20 Mar 2020 19:32:02 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:32:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:32:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Fri, 20 Mar 2020 19:32:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output
# Fri, 20 Mar 2020 19:32:04 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 20 Mar 2020 19:32:04 GMT
COPY dir:0d0cedab2fbb7208b9d81afa78e9f15b12b71232224a2fe9753c00b7b72bd72e in /opt/ibm/helpers/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Fri, 20 Mar 2020 19:32:06 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 20 Mar 2020 19:32:06 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:32:06 GMT
USER 1001
# Fri, 20 Mar 2020 19:32:06 GMT
EXPOSE 9080 9443
# Fri, 20 Mar 2020 19:32:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 20 Mar 2020 19:32:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 20 Mar 2020 19:32:10 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 20 Mar 2020 19:35:01 GMT
# ARGS: REPOSITORIES_PROPERTIES=
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 20 Mar 2020 19:35:01 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
```

-	Layers:
	-	`sha256:765ce743592771b94ad8ff27e281e66c13f6039962c7dde4dbe47123081e015b`  
		Last Modified: Mon, 16 Mar 2020 15:38:41 GMT  
		Size: 27.1 MB (27122453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dc9c4739090a3d2f7265f1f8184b1cbd8ae133b863f8aa93ec5cf1761ee7a5`  
		Last Modified: Fri, 20 Mar 2020 18:39:35 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a5b698281c077f48fc598e698f0619e4d00a2fedc1832fc95e9cf281408f63`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaebe599891b1e1befc10d752a117cc5615ec2dd3913d399fd66e26e0cace3e5`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f829150bc8a53a37ac17eb34838fa33c990881a4031bc650a9dae26b3f7880e`  
		Last Modified: Fri, 20 Mar 2020 19:09:23 GMT  
		Size: 3.0 MB (2992132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17b9ccc4baf3a1ffa517a03c7c3d01900136b128b36a83558c67c42e6c1cbaa`  
		Last Modified: Fri, 20 Mar 2020 19:09:35 GMT  
		Size: 118.8 MB (118756706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5011972f1876d464fb62206211a5b5e162ba2603bf20fc4cd0f2b4ffd311cd9`  
		Last Modified: Fri, 20 Mar 2020 19:39:16 GMT  
		Size: 13.6 MB (13600436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5395b713d5baa0917182ca82077b6fa2a0c51789907f96cbb12455586d9fa9b`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389324a3d9489b2fbcd5946f9d24285c0171c3218470e4a5e2d45c731cefc522`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 3.5 KB (3515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38ea596499e1f23ce426826250984869e92da50aec5845a6233a76d7764bfd1`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea3197b55235384f836e31a605c460f6cb7196f68dc29c65640738d8aa50188`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 57.4 KB (57426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683f76bf565cdb9e59c325f24357eb6b164555ed8629a4b8383448239608966d`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 4.4 KB (4358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd2560c76831311d13d197b4784e0826f6ffae62e3b9a22d2fa5675b9b71a2`  
		Last Modified: Fri, 20 Mar 2020 19:39:42 GMT  
		Size: 186.6 MB (186634496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891aa2b3e904f8f514677372187983ac12c98c209c433ab5bf0862e09d6f4ef`  
		Last Modified: Fri, 20 Mar 2020 19:39:20 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:faecb180eab0cf2e7ef66b023b667894577ba036211d2ecfe90253d136799327
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.0 MB (415020984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2632640bf1740b9f968ae52aa680b98fa04477aab0660c8baf5b8fddf79bf0a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:57:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 14:58:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:58:33 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 14:59:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 14:59:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:07:09 GMT
ARG VERBOSE=false
# Sat, 27 Mar 2021 05:07:11 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:36:22 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 22:36:27 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 22:36:31 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 22:36:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 22:36:37 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 22:36:41 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 22:36:46 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 22:38:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 22:38:05 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 22:38:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 22:38:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:38:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 22:38:41 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 22:38:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 22:39:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 22:39:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 22:39:38 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 22 Apr 2021 22:39:41 GMT
USER 1001
# Thu, 22 Apr 2021 22:39:45 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 22:39:51 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 22:39:55 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 22:43:49 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:43:55 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 22:48:08 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 22:48:12 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 22:49:35 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a8b760dceb1369716f09f0677ac6e4c109c24e134a9c883c7e48e1ee0d081`  
		Last Modified: Fri, 26 Mar 2021 15:03:04 GMT  
		Size: 3.1 MB (3082734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c129b1161496dd5f093240bbcc3a8117babb3970d1b268b5ef2a3b583cf288`  
		Last Modified: Fri, 26 Mar 2021 15:03:19 GMT  
		Size: 130.4 MB (130406650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec06bab51d83666979940922b947a720f6acaca816d2bf3cd332e567591afa4b`  
		Last Modified: Thu, 22 Apr 2021 23:13:03 GMT  
		Size: 14.1 MB (14062057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7f4311425eb37ef28297f5763e749844d439a78264d4863390508759094d6`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1685eb89d16b4bfbe9ff198cfccf641c1de3b8ea23ef56df88b431fed4260572`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 9.6 KB (9557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2045df8ec68a9c233ea9c9dcb3fb5568ea59166bb9912373e550945f7c42c1f`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc56667d904c50234135b3bfefa6630c14e255a6fbd7ee3143d06f8aac839ab9`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 10.6 KB (10553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5451ef86b75da4eaad3a9248b4b2158b6aca3cb0a19da6c9dfc7a955e8de2038`  
		Last Modified: Thu, 22 Apr 2021 23:12:59 GMT  
		Size: 5.3 MB (5327202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbb2811058d1ddf7c93605f52b4f92cf27c033ae5b026fb74b7584705122c15`  
		Last Modified: Thu, 22 Apr 2021 23:13:48 GMT  
		Size: 213.0 MB (212960397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab321d9643cb04efbdeaff3e7e94f91bd291323f304fc7b2943c5578468939e`  
		Last Modified: Thu, 22 Apr 2021 23:13:26 GMT  
		Size: 953.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edfcc0e4989bb4f0adce15dd3e622084b8b2c6ea9f85223785b1f7bcd097a5d`  
		Last Modified: Thu, 22 Apr 2021 23:13:31 GMT  
		Size: 18.7 MB (18735600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:1813d2e44e1f79784ab44778359fd80a47b37726d4ded32db082ca08eb72f80f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.0 MB (411023034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1109636c471215912302d8affaad06caa663cedee902a569c14ebc0e70e6a9a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:25:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 23 Apr 2021 22:25:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:25:17 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 23 Apr 2021 22:26:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 23 Apr 2021 22:26:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:16:58 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:16:58 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:16:59 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Fri, 23 Apr 2021 23:17:00 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Fri, 23 Apr 2021 23:17:00 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Fri, 23 Apr 2021 23:17:01 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:17:02 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Fri, 23 Apr 2021 23:17:02 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:17:03 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:17:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:17:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:17:21 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Fri, 23 Apr 2021 23:17:21 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:17:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:17:24 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:17:25 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:17:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:17:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:17:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:17:42 GMT
USER 1001
# Fri, 23 Apr 2021 23:17:42 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:17:43 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:17:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 23 Apr 2021 23:18:44 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:18:45 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 23 Apr 2021 23:22:46 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 23 Apr 2021 23:23:00 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 23 Apr 2021 23:23:44 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93b87da546ac7aa6705cd2f20bfe70cf04793ac73561e5dd8c579af88754aec`  
		Last Modified: Fri, 23 Apr 2021 22:28:41 GMT  
		Size: 2.7 MB (2676643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268462fc02d2bd9da227784f5f243759923a14cefb3648739ca02e8fa7d63ee7`  
		Last Modified: Fri, 23 Apr 2021 22:28:50 GMT  
		Size: 128.1 MB (128065984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895091e75a5c1ee863c074a41c334973d986bb55cef3d4ba2f8267a2887f8336`  
		Last Modified: Fri, 23 Apr 2021 23:53:50 GMT  
		Size: 14.1 MB (14061390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26d2145efe41abadeb2694f43164f1a155e500e85bf004da26812cd8532de7f`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1dc41aa938b0af86dfd6446147e4484cb5d6bad6e84eb2edb074790b0615a1`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 9.6 KB (9556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0e2666f7e25fefd1dfbbb522189283388626a78a6993958a175bfe3d453daa`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1422da1f78c4ff3f196f908ccd43d884e84e4586193eab1bfe59df39b352b130`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 10.5 KB (10540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a848b971c7539a51ff9771c57f7df448cc5b960c0be0fa5b3c3b547e8589c`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 5.9 MB (5924580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a29d9ef14335af914d1a4155de231f338e3649b1e962477e8f3c3007227195`  
		Last Modified: Fri, 23 Apr 2021 23:54:16 GMT  
		Size: 213.6 MB (213555213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85098d48d9a85bbbdc1b5f863692bf7b326b94c5f44d091ff39e53fb34a41cc`  
		Last Modified: Fri, 23 Apr 2021 23:54:05 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1e656c995305a66ce28c668c88b221183600d735978d891b72351644e890c2`  
		Last Modified: Fri, 23 Apr 2021 23:54:08 GMT  
		Size: 21.4 MB (21363413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:8ae8aa183b83bb2caf4e9508d9049825f2b3067e4a713de5f3e21b89187911e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:35cc2096f3510a3db928f854c16a9bedad246d1252f311c839f1c572d9c73dff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.6 MB (329563878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a13fac28833e00b5e3a59ae871ccdd0fbdf78ae2ea63171016753dc05b77a32`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 01:29:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 01:29:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:32:52 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:10 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 21:40:48 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:40:48 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:48 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 21:40:49 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 21:40:49 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 21:40:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:40:49 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 21:40:49 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:40:49 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:40:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:40:58 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:40:58 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 21:40:58 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:41:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:41:00 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:41:00 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:41:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:41:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:41:09 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 22 Apr 2021 21:41:09 GMT
USER 1001
# Thu, 22 Apr 2021 21:41:10 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:41:10 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:41:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 21:44:55 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:44:55 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 21:47:40 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 21:47:41 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 21:48:15 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04b772c31f76720583412a2507c5c53889985db45169a85f0d3cd7f842e041a`  
		Last Modified: Sat, 03 Apr 2021 01:39:30 GMT  
		Size: 16.0 MB (16032891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf71362343a962febc8c6ce8c4fd12d961c5712407993471f60ac0e5d43415e`  
		Last Modified: Mon, 19 Apr 2021 18:30:17 GMT  
		Size: 42.4 MB (42440313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9163852ff25e45c3b95c7b759a719b91afa29724136e68d1cf7f822c034c4df`  
		Last Modified: Mon, 19 Apr 2021 18:30:04 GMT  
		Size: 4.0 MB (4025359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a723eb5427857d3e6f939a462cbbaeedb1b248662076fe72f2fab621d9acc3`  
		Last Modified: Thu, 22 Apr 2021 21:57:15 GMT  
		Size: 14.2 MB (14160245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0598dd9101a4447350e39fc9445131bdeb5a9bee7fc233879f0451c08a79fe`  
		Last Modified: Thu, 22 Apr 2021 21:57:12 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf163d48e000642c258afeea2bb09c0cca8829f72fcd792c97840c181f7331f8`  
		Last Modified: Thu, 22 Apr 2021 21:57:12 GMT  
		Size: 9.6 KB (9550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5906189dfc1fa00888b59c4cefad5a2f4aa3085bcc6da5d37e63197585a231c`  
		Last Modified: Thu, 22 Apr 2021 21:57:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062608db9cb7d8e8fc2dfa23464525e84b5d5fe1bc979194b937d8b2a4de74a6`  
		Last Modified: Thu, 22 Apr 2021 21:57:11 GMT  
		Size: 10.5 KB (10531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2d74ce76564c5e8a6dafde72882602b446b3d3d81d620c5b1f08232a5a019`  
		Last Modified: Thu, 22 Apr 2021 21:57:11 GMT  
		Size: 2.6 MB (2555007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2717086accd7d50a5527b2b70f1177f08e904718f5388f702983ce093761304`  
		Last Modified: Thu, 22 Apr 2021 21:58:02 GMT  
		Size: 207.7 MB (207669936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59e20e338e249cff7c3435973456929f13dfea41138604d3fe1696e479dc61`  
		Last Modified: Thu, 22 Apr 2021 21:57:50 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455eb33d7a0b34ae7cec9f9f41505c10dd6db2bd14f0f792b193a312a1c64b9e`  
		Last Modified: Thu, 22 Apr 2021 21:57:53 GMT  
		Size: 14.1 MB (14088088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:07540a882ea5483563b694c0dad8ae082abd9ae8c39c96be69a8730b843f0804
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.5 MB (334547474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c92dca05464955a0c79c7e5f82f7489fc4727cf3a74c5cea077620bb7a4fd42f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 05:41:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 05:43:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 05:51:38 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:15 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 22:40:19 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:40:26 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:40:30 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 22:40:33 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 22:40:37 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 22:40:40 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 22:40:45 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 22:40:52 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 22:40:56 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 22:41:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 22:41:46 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 22:41:56 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 22:42:04 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:42:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 22:42:23 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 22:42:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 22:42:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 22:43:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 22:43:11 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 22 Apr 2021 22:43:15 GMT
USER 1001
# Thu, 22 Apr 2021 22:43:19 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 22:43:24 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 22:43:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 22:49:54 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:49:59 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 22:53:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 22:54:02 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 22:55:14 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3147f9d7021e4b4f874d531cd0d820bd489543f00c894d4d9df8f2c1b0777d2b`  
		Last Modified: Sat, 03 Apr 2021 06:01:07 GMT  
		Size: 17.2 MB (17208203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422c588ac4abf48f1a915be1f8f943b1dbc48565bc9f3816ef2bc82f6eb2b9e9`  
		Last Modified: Mon, 19 Apr 2021 18:33:46 GMT  
		Size: 43.3 MB (43277555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e121c025bd5ea767e5c45ee767dc2033229a9d9fb8d83a441bd012a380fd`  
		Last Modified: Mon, 19 Apr 2021 18:33:34 GMT  
		Size: 3.3 MB (3280395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6929ab0e248a58c5b49948573b1127df1bcbe68796a5e21814a4c9e4e28f6ebf`  
		Last Modified: Thu, 22 Apr 2021 23:13:18 GMT  
		Size: 14.2 MB (14161071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2588e073d28ae56c3b8dfd39e5a1d6dccae837dd371077e43397444ffb8ff1e`  
		Last Modified: Thu, 22 Apr 2021 23:13:11 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a98cf9a7933225976737f1a20308355729c508995402133840fcc479f27d43`  
		Last Modified: Thu, 22 Apr 2021 23:13:12 GMT  
		Size: 9.6 KB (9551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac8f8e29ad8d0df0b59f8076e79f3af0ff5d168e821f3cd7ac29b1d58ab08f1`  
		Last Modified: Thu, 22 Apr 2021 23:13:11 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1f252245d30a42990c0c73190e7139531fa283f5d7ee5ebd4df55dfe374412`  
		Last Modified: Thu, 22 Apr 2021 23:13:11 GMT  
		Size: 10.5 KB (10543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef9dd9d762820f249356fcd609a933f771ea6d3958711f43e56650e6507342c`  
		Last Modified: Thu, 22 Apr 2021 23:13:12 GMT  
		Size: 2.5 MB (2452650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8319ed53797eb366322fe8e99f98580a1331d4816d5144074d9cadca6cd789c`  
		Last Modified: Thu, 22 Apr 2021 23:14:21 GMT  
		Size: 207.7 MB (207671859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf42350fcce58dfd0beca958548225d94e2ffb95de42637e27781977f3842d2`  
		Last Modified: Thu, 22 Apr 2021 23:14:00 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d061bc3e9092696be441f9b782f5d6cbfaf1b296a48f5c8469817146c5386`  
		Last Modified: Thu, 22 Apr 2021 23:14:03 GMT  
		Size: 13.2 MB (13192654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0d02e361435df46fff35ebc173579ebb1dafbc0713fa6fa5882156f0ac9abb76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.6 MB (326645376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c382f67d2996379923080d0c01ae3039c6ef3b9f1e0b452d32958d81cd7e7487`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:03:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 22:04:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:10:11 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Fri, 23 Apr 2021 22:11:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 23 Apr 2021 22:11:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 22:11:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 23 Apr 2021 22:12:20 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 23 Apr 2021 23:17:55 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:17:56 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:17:56 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Fri, 23 Apr 2021 23:17:57 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Fri, 23 Apr 2021 23:17:57 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Fri, 23 Apr 2021 23:17:58 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:17:59 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Fri, 23 Apr 2021 23:17:59 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:18:00 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:18:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:18:15 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:18:16 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Fri, 23 Apr 2021 23:18:16 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:18:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:18:19 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:18:19 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:18:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:18:32 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:18:33 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Fri, 23 Apr 2021 23:18:34 GMT
USER 1001
# Fri, 23 Apr 2021 23:18:35 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:18:36 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:18:36 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 23 Apr 2021 23:24:07 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:24:07 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 23 Apr 2021 23:28:09 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 23 Apr 2021 23:28:21 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 23 Apr 2021 23:29:08 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bab416938acf6dd045c9fc9097e5768c61b5899b07d110ab3844f447e12b113`  
		Last Modified: Fri, 23 Apr 2021 22:19:05 GMT  
		Size: 15.7 MB (15741779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0273d3bc7cd55960a36b00d19e8d51f8bbeed03d24fd8d551c957fc19ef079b`  
		Last Modified: Fri, 23 Apr 2021 22:22:19 GMT  
		Size: 42.0 MB (41951613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95422aa686364d2877a279281f6eb1157805fa8516aa976b06ce8889dc9f932`  
		Last Modified: Fri, 23 Apr 2021 22:22:13 GMT  
		Size: 3.8 MB (3836026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f024126ee5e04e37dd48573fe2e6aefd2d98012df116b366e0aef9fa63b8ba93`  
		Last Modified: Fri, 23 Apr 2021 23:54:00 GMT  
		Size: 14.2 MB (14160729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a63a9d57fd3b2ed838f0044559d5cfa241eab25d7626378b2fd1c5463947a9`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 687.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62def58659c4a5a6fd3cde1c4245691f62a7d197ac87536975c7c888e8fd5ff`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 9.6 KB (9551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288fec31697eb659f1a7285ca37ce8460c07bd8485fdb21628ff246a6661660d`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bce08718a41817d4e1e9dd6bb83ac83f3a1c3014753a04447805c257e51a9c3`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 10.5 KB (10544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3096c60acccc8db5e2ef0df733a4693cf8068658a1fc8af639461c112c1589a`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 2.5 MB (2491647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d29297ab00722488619fd9526e89b49277ed66bac34206e8f7e2cb0917e1945`  
		Last Modified: Fri, 23 Apr 2021 23:54:35 GMT  
		Size: 207.7 MB (207671747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b7a66a256bd33f418c1622886d5384d5a5abc02e2c3b042d528a7153211728`  
		Last Modified: Fri, 23 Apr 2021 23:54:24 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba111cf88078cf3a5f862c69d813cf4940c21337daefa46d9c6a9818aae58d8e`  
		Last Modified: Fri, 23 Apr 2021 23:54:26 GMT  
		Size: 13.6 MB (13632445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel`

```console
$ docker pull websphere-liberty@sha256:099c345c922421a25266ed9f1db4540e9e373709123936993ae3392381515d3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:f528365190e853e1ffbc72c586114358fb2eb6e0117c4134f68e0e57894f6f24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180293270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79615f972bc823a2954599784f3311d9cd8c7d4e5bc2ee82a917c4f753326937`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:30:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 09:31:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:31:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 09:31:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 09:31:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:31:17 GMT
ARG VERBOSE=false
# Fri, 26 Mar 2021 21:31:18 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:06 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 21:40:06 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 21:40:06 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 21:40:06 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:40:06 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 21:40:07 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:40:07 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:40:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:40:24 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:40:24 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 21:40:24 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:40:26 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:40:26 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:40:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:40:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:40:38 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 22 Apr 2021 21:40:38 GMT
USER 1001
# Thu, 22 Apr 2021 21:40:39 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:40:39 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:40:39 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4764ed71d2900c9874838108e377eb8821088502d5504fadeb080e5dd1a3e65d`  
		Last Modified: Fri, 26 Mar 2021 09:35:47 GMT  
		Size: 3.0 MB (2958415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf5000c541da177b7cfe59bf3ff8cb271529f443ee224bf88989910e9a2abb1`  
		Last Modified: Fri, 26 Mar 2021 09:36:01 GMT  
		Size: 130.8 MB (130805802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df46370333075337eb25c08aa74c706467351aa5abe9711e870aa5e647baaf`  
		Last Modified: Thu, 22 Apr 2021 21:57:02 GMT  
		Size: 14.1 MB (14061162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d854faca6db468012fcae8e445cd69affeb82c5efbb89ac2b53b719cb4eabd`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f56d571437c689e2188bb2653cbbaf3ef56de28093fd63e3229a142d9d87fa`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 9.6 KB (9556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fde75a052b81ad9ca202510ebedb5083754ed163d499a6f28f1be76b6615ad`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610a90e750f1b7eb794e24a2970acb3b9f79a569ed064d70771895e2cf5c4795`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 10.5 KB (10544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3782c27b14b1eea6ec7f8a3c56182ccbf3a0db0e5a00cb4aad829f8b16f628b1`  
		Last Modified: Thu, 22 Apr 2021 21:56:59 GMT  
		Size: 5.7 MB (5734998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; 386

```console
$ docker pull websphere-liberty@sha256:21c2835a021b91c09268f12dc8f3c61f590c1b34d7669aeacf3792d83a7ef016
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162573580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e89243446a76e85ea4bf274dd0ad9e6fd0e763e50ced541577b62bee7dfcb74`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:38:55 GMT
ADD file:d859d389e38b7ac70fd56f97e38d52a77b58e72b96237a4302d1984cdd912a55 in / 
# Fri, 20 Mar 2020 18:38:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:38:57 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:38:58 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:38:58 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:06:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 20 Mar 2020 19:06:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:06:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp6
# Fri, 20 Mar 2020 19:07:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='87f9d45b7e1fa65ec018479f3ca7da69a03b52b0da10b8d1555142eec8ab0093';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='b5f825047c9bb5d360fb83694f12e17b1a5a15abf94ac82cd0a3aea32c9a361c';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f3c04cd07ef269c24373840eae6f59c7db7a16d2e206d393ba93efa6dbb8d74f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2bbefda96f7d1a5f1694893961e92ccc59dfa50375ae5450675d7a4213d5812e';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='d5b0508d53d1c7382c06f5bc1daf3d57c19c70d851e86e6b1162bcd93f616f7e';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 20 Mar 2020 19:07:26 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:31:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433
# Fri, 20 Mar 2020 19:31:53 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Fri, 20 Mar 2020 19:31:53 GMT
ARG LIBERTY_URL
# Fri, 20 Mar 2020 19:31:53 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 20 Mar 2020 19:32:02 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:32:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:32:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Fri, 20 Mar 2020 19:32:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output
# Fri, 20 Mar 2020 19:32:04 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 20 Mar 2020 19:32:04 GMT
COPY dir:0d0cedab2fbb7208b9d81afa78e9f15b12b71232224a2fe9753c00b7b72bd72e in /opt/ibm/helpers/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Fri, 20 Mar 2020 19:32:06 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 20 Mar 2020 19:32:06 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:32:06 GMT
USER 1001
# Fri, 20 Mar 2020 19:32:06 GMT
EXPOSE 9080 9443
# Fri, 20 Mar 2020 19:32:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 20 Mar 2020 19:32:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:765ce743592771b94ad8ff27e281e66c13f6039962c7dde4dbe47123081e015b`  
		Last Modified: Mon, 16 Mar 2020 15:38:41 GMT  
		Size: 27.1 MB (27122453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dc9c4739090a3d2f7265f1f8184b1cbd8ae133b863f8aa93ec5cf1761ee7a5`  
		Last Modified: Fri, 20 Mar 2020 18:39:35 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a5b698281c077f48fc598e698f0619e4d00a2fedc1832fc95e9cf281408f63`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaebe599891b1e1befc10d752a117cc5615ec2dd3913d399fd66e26e0cace3e5`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f829150bc8a53a37ac17eb34838fa33c990881a4031bc650a9dae26b3f7880e`  
		Last Modified: Fri, 20 Mar 2020 19:09:23 GMT  
		Size: 3.0 MB (2992132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17b9ccc4baf3a1ffa517a03c7c3d01900136b128b36a83558c67c42e6c1cbaa`  
		Last Modified: Fri, 20 Mar 2020 19:09:35 GMT  
		Size: 118.8 MB (118756706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5011972f1876d464fb62206211a5b5e162ba2603bf20fc4cd0f2b4ffd311cd9`  
		Last Modified: Fri, 20 Mar 2020 19:39:16 GMT  
		Size: 13.6 MB (13600436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5395b713d5baa0917182ca82077b6fa2a0c51789907f96cbb12455586d9fa9b`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389324a3d9489b2fbcd5946f9d24285c0171c3218470e4a5e2d45c731cefc522`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 3.5 KB (3515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38ea596499e1f23ce426826250984869e92da50aec5845a6233a76d7764bfd1`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea3197b55235384f836e31a605c460f6cb7196f68dc29c65640738d8aa50188`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 57.4 KB (57426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683f76bf565cdb9e59c325f24357eb6b164555ed8629a4b8383448239608966d`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 4.4 KB (4358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:6322cd5c750764e7efee92c0f43a9cdffade75d0c8480ab4c7c24ed8c5b3af2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.3 MB (183324034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc735b0a89ae88f071398c01160e7248b957a412c35d93bb33bfbc5575693f9c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:57:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 14:58:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:58:33 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 14:59:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 14:59:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:07:09 GMT
ARG VERBOSE=false
# Sat, 27 Mar 2021 05:07:11 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:36:22 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 22:36:27 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 22:36:31 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 22:36:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 22:36:37 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 22:36:41 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 22:36:46 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 22:38:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 22:38:05 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 22:38:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 22:38:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:38:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 22:38:41 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 22:38:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 22:39:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 22:39:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 22:39:38 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 22 Apr 2021 22:39:41 GMT
USER 1001
# Thu, 22 Apr 2021 22:39:45 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 22:39:51 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 22:39:55 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a8b760dceb1369716f09f0677ac6e4c109c24e134a9c883c7e48e1ee0d081`  
		Last Modified: Fri, 26 Mar 2021 15:03:04 GMT  
		Size: 3.1 MB (3082734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c129b1161496dd5f093240bbcc3a8117babb3970d1b268b5ef2a3b583cf288`  
		Last Modified: Fri, 26 Mar 2021 15:03:19 GMT  
		Size: 130.4 MB (130406650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec06bab51d83666979940922b947a720f6acaca816d2bf3cd332e567591afa4b`  
		Last Modified: Thu, 22 Apr 2021 23:13:03 GMT  
		Size: 14.1 MB (14062057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7f4311425eb37ef28297f5763e749844d439a78264d4863390508759094d6`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1685eb89d16b4bfbe9ff198cfccf641c1de3b8ea23ef56df88b431fed4260572`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 9.6 KB (9557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2045df8ec68a9c233ea9c9dcb3fb5568ea59166bb9912373e550945f7c42c1f`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc56667d904c50234135b3bfefa6630c14e255a6fbd7ee3143d06f8aac839ab9`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 10.6 KB (10553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5451ef86b75da4eaad3a9248b4b2158b6aca3cb0a19da6c9dfc7a955e8de2038`  
		Last Modified: Thu, 22 Apr 2021 23:12:59 GMT  
		Size: 5.3 MB (5327202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0d7dafd042d0d2cc8eb4580d0db30ada5047e8848c332172235044b128158d2f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176103462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a099f0ae43c0fd8c3e964020f65971f96b5f6988450d42231f7333bb9b4fb8f2`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:25:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 23 Apr 2021 22:25:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:25:17 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 23 Apr 2021 22:26:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 23 Apr 2021 22:26:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:16:58 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:16:58 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:16:59 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Fri, 23 Apr 2021 23:17:00 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Fri, 23 Apr 2021 23:17:00 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Fri, 23 Apr 2021 23:17:01 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:17:02 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Fri, 23 Apr 2021 23:17:02 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:17:03 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:17:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:17:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:17:21 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Fri, 23 Apr 2021 23:17:21 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:17:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:17:24 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:17:25 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:17:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:17:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:17:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:17:42 GMT
USER 1001
# Fri, 23 Apr 2021 23:17:42 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:17:43 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:17:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93b87da546ac7aa6705cd2f20bfe70cf04793ac73561e5dd8c579af88754aec`  
		Last Modified: Fri, 23 Apr 2021 22:28:41 GMT  
		Size: 2.7 MB (2676643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268462fc02d2bd9da227784f5f243759923a14cefb3648739ca02e8fa7d63ee7`  
		Last Modified: Fri, 23 Apr 2021 22:28:50 GMT  
		Size: 128.1 MB (128065984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895091e75a5c1ee863c074a41c334973d986bb55cef3d4ba2f8267a2887f8336`  
		Last Modified: Fri, 23 Apr 2021 23:53:50 GMT  
		Size: 14.1 MB (14061390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26d2145efe41abadeb2694f43164f1a155e500e85bf004da26812cd8532de7f`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1dc41aa938b0af86dfd6446147e4484cb5d6bad6e84eb2edb074790b0615a1`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 9.6 KB (9556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0e2666f7e25fefd1dfbbb522189283388626a78a6993958a175bfe3d453daa`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1422da1f78c4ff3f196f908ccd43d884e84e4586193eab1bfe59df39b352b130`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 10.5 KB (10540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a848b971c7539a51ff9771c57f7df448cc5b960c0be0fa5b3c3b547e8589c`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 5.9 MB (5924580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:fe1abe1b8727e22b222d63ad4486ef6da1e3018131b94234fe5977ee4b59a8f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:089c25ea4ac42c4cedb0b974d8cf29185eb9c3ec4e86fa10817a8afa5de7f601
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107804910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98fb4f6747d498676b24bc7bf8aa4905b802d1f2ed2d3b27bce67a59d00748c5`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 01:29:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 01:29:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:32:52 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:34 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:10 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 21:40:48 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:40:48 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:48 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 21:40:49 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 21:40:49 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 21:40:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:40:49 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 21:40:49 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:40:49 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:40:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:40:58 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:40:58 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 21:40:58 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:41:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:41:00 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:41:00 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:41:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:41:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:41:09 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 22 Apr 2021 21:41:09 GMT
USER 1001
# Thu, 22 Apr 2021 21:41:10 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:41:10 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:41:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04b772c31f76720583412a2507c5c53889985db45169a85f0d3cd7f842e041a`  
		Last Modified: Sat, 03 Apr 2021 01:39:30 GMT  
		Size: 16.0 MB (16032891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf71362343a962febc8c6ce8c4fd12d961c5712407993471f60ac0e5d43415e`  
		Last Modified: Mon, 19 Apr 2021 18:30:17 GMT  
		Size: 42.4 MB (42440313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9163852ff25e45c3b95c7b759a719b91afa29724136e68d1cf7f822c034c4df`  
		Last Modified: Mon, 19 Apr 2021 18:30:04 GMT  
		Size: 4.0 MB (4025359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a723eb5427857d3e6f939a462cbbaeedb1b248662076fe72f2fab621d9acc3`  
		Last Modified: Thu, 22 Apr 2021 21:57:15 GMT  
		Size: 14.2 MB (14160245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0598dd9101a4447350e39fc9445131bdeb5a9bee7fc233879f0451c08a79fe`  
		Last Modified: Thu, 22 Apr 2021 21:57:12 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf163d48e000642c258afeea2bb09c0cca8829f72fcd792c97840c181f7331f8`  
		Last Modified: Thu, 22 Apr 2021 21:57:12 GMT  
		Size: 9.6 KB (9550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5906189dfc1fa00888b59c4cefad5a2f4aa3085bcc6da5d37e63197585a231c`  
		Last Modified: Thu, 22 Apr 2021 21:57:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062608db9cb7d8e8fc2dfa23464525e84b5d5fe1bc979194b937d8b2a4de74a6`  
		Last Modified: Thu, 22 Apr 2021 21:57:11 GMT  
		Size: 10.5 KB (10531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2d74ce76564c5e8a6dafde72882602b446b3d3d81d620c5b1f08232a5a019`  
		Last Modified: Thu, 22 Apr 2021 21:57:11 GMT  
		Size: 2.6 MB (2555007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:db1df505afa055570fd1730ad5546e03de17d85d4e49d3758b8f46f2d706a977
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113682013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77818b750cad7803852ce86ef76b32a4d32276ef03279d867bedee73e1663156`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 05:41:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 05:43:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 05:51:38 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Mon, 19 Apr 2021 18:22:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 19 Apr 2021 18:22:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Apr 2021 18:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 19 Apr 2021 18:23:15 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 22 Apr 2021 22:40:19 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:40:26 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:40:30 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 22:40:33 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 22:40:37 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 22:40:40 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 22:40:45 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 22:40:52 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 22:40:56 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 22:41:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 22:41:46 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 22:41:56 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 22:42:04 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:42:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 22:42:23 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 22:42:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 22:42:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 22:43:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 22:43:11 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 22 Apr 2021 22:43:15 GMT
USER 1001
# Thu, 22 Apr 2021 22:43:19 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 22:43:24 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 22:43:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3147f9d7021e4b4f874d531cd0d820bd489543f00c894d4d9df8f2c1b0777d2b`  
		Last Modified: Sat, 03 Apr 2021 06:01:07 GMT  
		Size: 17.2 MB (17208203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422c588ac4abf48f1a915be1f8f943b1dbc48565bc9f3816ef2bc82f6eb2b9e9`  
		Last Modified: Mon, 19 Apr 2021 18:33:46 GMT  
		Size: 43.3 MB (43277555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e121c025bd5ea767e5c45ee767dc2033229a9d9fb8d83a441bd012a380fd`  
		Last Modified: Mon, 19 Apr 2021 18:33:34 GMT  
		Size: 3.3 MB (3280395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6929ab0e248a58c5b49948573b1127df1bcbe68796a5e21814a4c9e4e28f6ebf`  
		Last Modified: Thu, 22 Apr 2021 23:13:18 GMT  
		Size: 14.2 MB (14161071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2588e073d28ae56c3b8dfd39e5a1d6dccae837dd371077e43397444ffb8ff1e`  
		Last Modified: Thu, 22 Apr 2021 23:13:11 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a98cf9a7933225976737f1a20308355729c508995402133840fcc479f27d43`  
		Last Modified: Thu, 22 Apr 2021 23:13:12 GMT  
		Size: 9.6 KB (9551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac8f8e29ad8d0df0b59f8076e79f3af0ff5d168e821f3cd7ac29b1d58ab08f1`  
		Last Modified: Thu, 22 Apr 2021 23:13:11 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1f252245d30a42990c0c73190e7139531fa283f5d7ee5ebd4df55dfe374412`  
		Last Modified: Thu, 22 Apr 2021 23:13:11 GMT  
		Size: 10.5 KB (10543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef9dd9d762820f249356fcd609a933f771ea6d3958711f43e56650e6507342c`  
		Last Modified: Thu, 22 Apr 2021 23:13:12 GMT  
		Size: 2.5 MB (2452650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:7da2d996a0edd7759eef333322be612a3aa048d1c48ffec09bef5d1d8aca195e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105340236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0450ad9b23e181ff9223541e51f3bd15bdc098a0b0e011fda20432f21f2b5467`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:03:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 22:04:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:10:11 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Fri, 23 Apr 2021 22:11:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='5d2b2939637f999a1910d5cc0fb3d96756125941e5f8b9e3003635aa863664b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='2ff9f50d6ffc345434703c43a1d67ac6d3d054b5d4925b4b73a3ce51b02940e5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7e5f97071f8b86c22c36ddfd7f821c3e8ec531c1128e2e6c931b2e64118a517a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 23 Apr 2021 22:11:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 22:11:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 23 Apr 2021 22:12:20 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 23 Apr 2021 23:17:55 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:17:56 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:17:56 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Fri, 23 Apr 2021 23:17:57 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Fri, 23 Apr 2021 23:17:57 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Fri, 23 Apr 2021 23:17:58 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:17:59 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Fri, 23 Apr 2021 23:17:59 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:18:00 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:18:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:18:15 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:18:16 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Fri, 23 Apr 2021 23:18:16 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:18:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:18:19 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:18:19 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:18:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:18:32 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:18:33 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Fri, 23 Apr 2021 23:18:34 GMT
USER 1001
# Fri, 23 Apr 2021 23:18:35 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:18:36 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:18:36 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bab416938acf6dd045c9fc9097e5768c61b5899b07d110ab3844f447e12b113`  
		Last Modified: Fri, 23 Apr 2021 22:19:05 GMT  
		Size: 15.7 MB (15741779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0273d3bc7cd55960a36b00d19e8d51f8bbeed03d24fd8d551c957fc19ef079b`  
		Last Modified: Fri, 23 Apr 2021 22:22:19 GMT  
		Size: 42.0 MB (41951613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95422aa686364d2877a279281f6eb1157805fa8516aa976b06ce8889dc9f932`  
		Last Modified: Fri, 23 Apr 2021 22:22:13 GMT  
		Size: 3.8 MB (3836026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f024126ee5e04e37dd48573fe2e6aefd2d98012df116b366e0aef9fa63b8ba93`  
		Last Modified: Fri, 23 Apr 2021 23:54:00 GMT  
		Size: 14.2 MB (14160729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a63a9d57fd3b2ed838f0044559d5cfa241eab25d7626378b2fd1c5463947a9`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 687.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62def58659c4a5a6fd3cde1c4245691f62a7d197ac87536975c7c888e8fd5ff`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 9.6 KB (9551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288fec31697eb659f1a7285ca37ce8460c07bd8485fdb21628ff246a6661660d`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bce08718a41817d4e1e9dd6bb83ac83f3a1c3014753a04447805c257e51a9c3`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 10.5 KB (10544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3096c60acccc8db5e2ef0df733a4693cf8068658a1fc8af639461c112c1589a`  
		Last Modified: Fri, 23 Apr 2021 23:53:57 GMT  
		Size: 2.5 MB (2491647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:latest`

```console
$ docker pull websphere-liberty@sha256:c57170761ec676e97a6a99f5004cc3080789d3b9f985247ff8cc1ecd50ff5c1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:latest` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:750da2549ddcfbd3e9ae2850b9ae2347adbb712410041faf8a02a81d635d2cde
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.8 MB (414810589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bfd08f9c2afdc6e2530607e9db350908221943ae7b3a387ed47fde3bad081c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:30:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 09:31:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:31:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 09:31:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 09:31:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 21:31:17 GMT
ARG VERBOSE=false
# Fri, 26 Mar 2021 21:31:18 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:06 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 21:40:06 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 21:40:06 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 21:40:06 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 21:40:06 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 21:40:07 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 21:40:07 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 21:40:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 21:40:24 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 21:40:24 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 21:40:24 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 21:40:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 21:40:26 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 21:40:26 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 21:40:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 21:40:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 21:40:38 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 22 Apr 2021 21:40:38 GMT
USER 1001
# Thu, 22 Apr 2021 21:40:39 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 21:40:39 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 21:40:39 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 21:41:13 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 21:41:13 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 21:44:16 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 21:44:16 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 21:44:52 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4764ed71d2900c9874838108e377eb8821088502d5504fadeb080e5dd1a3e65d`  
		Last Modified: Fri, 26 Mar 2021 09:35:47 GMT  
		Size: 3.0 MB (2958415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf5000c541da177b7cfe59bf3ff8cb271529f443ee224bf88989910e9a2abb1`  
		Last Modified: Fri, 26 Mar 2021 09:36:01 GMT  
		Size: 130.8 MB (130805802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df46370333075337eb25c08aa74c706467351aa5abe9711e870aa5e647baaf`  
		Last Modified: Thu, 22 Apr 2021 21:57:02 GMT  
		Size: 14.1 MB (14061162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d854faca6db468012fcae8e445cd69affeb82c5efbb89ac2b53b719cb4eabd`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f56d571437c689e2188bb2653cbbaf3ef56de28093fd63e3229a142d9d87fa`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 9.6 KB (9556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fde75a052b81ad9ca202510ebedb5083754ed163d499a6f28f1be76b6615ad`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610a90e750f1b7eb794e24a2970acb3b9f79a569ed064d70771895e2cf5c4795`  
		Last Modified: Thu, 22 Apr 2021 21:56:58 GMT  
		Size: 10.5 KB (10544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3782c27b14b1eea6ec7f8a3c56182ccbf3a0db0e5a00cb4aad829f8b16f628b1`  
		Last Modified: Thu, 22 Apr 2021 21:56:59 GMT  
		Size: 5.7 MB (5734998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f94a4feba9d432ba504a626d7c726342855fc5baffbda070b24e905aa4d6f2`  
		Last Modified: Thu, 22 Apr 2021 21:57:36 GMT  
		Size: 213.4 MB (213364505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f32f1e0b41195d19cb5b1bc063af6b2ebd037fee723a18c58cee092d68b465`  
		Last Modified: Thu, 22 Apr 2021 21:57:24 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926bbbd582bf41deb09392c6714bc00b03c3a35a16db042c445f171588d03f52`  
		Last Modified: Thu, 22 Apr 2021 21:57:28 GMT  
		Size: 21.2 MB (21151866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; 386

```console
$ docker pull websphere-liberty@sha256:c847143995aec30ca5d4526544d7c41ca7a42a8baf8195848864d0128e96ecf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.2 MB (349209019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d2c9374be56a63d6e35820fec8676f2d4ed2b9bdaf09a49c8545b039479bb7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:38:55 GMT
ADD file:d859d389e38b7ac70fd56f97e38d52a77b58e72b96237a4302d1984cdd912a55 in / 
# Fri, 20 Mar 2020 18:38:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:38:57 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:38:58 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:38:58 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:06:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 20 Mar 2020 19:06:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:06:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp6
# Fri, 20 Mar 2020 19:07:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='87f9d45b7e1fa65ec018479f3ca7da69a03b52b0da10b8d1555142eec8ab0093';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='b5f825047c9bb5d360fb83694f12e17b1a5a15abf94ac82cd0a3aea32c9a361c';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f3c04cd07ef269c24373840eae6f59c7db7a16d2e206d393ba93efa6dbb8d74f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2bbefda96f7d1a5f1694893961e92ccc59dfa50375ae5450675d7a4213d5812e';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='d5b0508d53d1c7382c06f5bc1daf3d57c19c70d851e86e6b1162bcd93f616f7e';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 20 Mar 2020 19:07:26 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:31:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433
# Fri, 20 Mar 2020 19:31:53 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Fri, 20 Mar 2020 19:31:53 GMT
ARG LIBERTY_URL
# Fri, 20 Mar 2020 19:31:53 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 20 Mar 2020 19:32:02 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:32:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:32:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Fri, 20 Mar 2020 19:32:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output
# Fri, 20 Mar 2020 19:32:04 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 20 Mar 2020 19:32:04 GMT
COPY dir:0d0cedab2fbb7208b9d81afa78e9f15b12b71232224a2fe9753c00b7b72bd72e in /opt/ibm/helpers/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Fri, 20 Mar 2020 19:32:06 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 20 Mar 2020 19:32:06 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:32:06 GMT
USER 1001
# Fri, 20 Mar 2020 19:32:06 GMT
EXPOSE 9080 9443
# Fri, 20 Mar 2020 19:32:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 20 Mar 2020 19:32:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 20 Mar 2020 19:32:10 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 20 Mar 2020 19:35:01 GMT
# ARGS: REPOSITORIES_PROPERTIES=
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 20 Mar 2020 19:35:01 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
```

-	Layers:
	-	`sha256:765ce743592771b94ad8ff27e281e66c13f6039962c7dde4dbe47123081e015b`  
		Last Modified: Mon, 16 Mar 2020 15:38:41 GMT  
		Size: 27.1 MB (27122453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dc9c4739090a3d2f7265f1f8184b1cbd8ae133b863f8aa93ec5cf1761ee7a5`  
		Last Modified: Fri, 20 Mar 2020 18:39:35 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a5b698281c077f48fc598e698f0619e4d00a2fedc1832fc95e9cf281408f63`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaebe599891b1e1befc10d752a117cc5615ec2dd3913d399fd66e26e0cace3e5`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f829150bc8a53a37ac17eb34838fa33c990881a4031bc650a9dae26b3f7880e`  
		Last Modified: Fri, 20 Mar 2020 19:09:23 GMT  
		Size: 3.0 MB (2992132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17b9ccc4baf3a1ffa517a03c7c3d01900136b128b36a83558c67c42e6c1cbaa`  
		Last Modified: Fri, 20 Mar 2020 19:09:35 GMT  
		Size: 118.8 MB (118756706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5011972f1876d464fb62206211a5b5e162ba2603bf20fc4cd0f2b4ffd311cd9`  
		Last Modified: Fri, 20 Mar 2020 19:39:16 GMT  
		Size: 13.6 MB (13600436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5395b713d5baa0917182ca82077b6fa2a0c51789907f96cbb12455586d9fa9b`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389324a3d9489b2fbcd5946f9d24285c0171c3218470e4a5e2d45c731cefc522`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 3.5 KB (3515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38ea596499e1f23ce426826250984869e92da50aec5845a6233a76d7764bfd1`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea3197b55235384f836e31a605c460f6cb7196f68dc29c65640738d8aa50188`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 57.4 KB (57426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683f76bf565cdb9e59c325f24357eb6b164555ed8629a4b8383448239608966d`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 4.4 KB (4358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd2560c76831311d13d197b4784e0826f6ffae62e3b9a22d2fa5675b9b71a2`  
		Last Modified: Fri, 20 Mar 2020 19:39:42 GMT  
		Size: 186.6 MB (186634496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891aa2b3e904f8f514677372187983ac12c98c209c433ab5bf0862e09d6f4ef`  
		Last Modified: Fri, 20 Mar 2020 19:39:20 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:faecb180eab0cf2e7ef66b023b667894577ba036211d2ecfe90253d136799327
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.0 MB (415020984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2632640bf1740b9f968ae52aa680b98fa04477aab0660c8baf5b8fddf79bf0a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:57:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 14:58:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:58:33 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 14:59:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 14:59:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 27 Mar 2021 05:07:09 GMT
ARG VERBOSE=false
# Sat, 27 Mar 2021 05:07:11 GMT
ARG OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:36:22 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Thu, 22 Apr 2021 22:36:27 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Thu, 22 Apr 2021 22:36:31 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Thu, 22 Apr 2021 22:36:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 22 Apr 2021 22:36:37 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Thu, 22 Apr 2021 22:36:41 GMT
ARG LIBERTY_URL
# Thu, 22 Apr 2021 22:36:46 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 22 Apr 2021 22:38:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Apr 2021 22:38:05 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Apr 2021 22:38:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Thu, 22 Apr 2021 22:38:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 22 Apr 2021 22:38:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 22 Apr 2021 22:38:41 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Thu, 22 Apr 2021 22:38:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 22 Apr 2021 22:39:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 22 Apr 2021 22:39:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 22 Apr 2021 22:39:38 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 22 Apr 2021 22:39:41 GMT
USER 1001
# Thu, 22 Apr 2021 22:39:45 GMT
EXPOSE 9080 9443
# Thu, 22 Apr 2021 22:39:51 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 22 Apr 2021 22:39:55 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 22 Apr 2021 22:43:49 GMT
ARG VERBOSE=false
# Thu, 22 Apr 2021 22:43:55 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 22 Apr 2021 22:48:08 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 22 Apr 2021 22:48:12 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 22 Apr 2021 22:49:35 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a8b760dceb1369716f09f0677ac6e4c109c24e134a9c883c7e48e1ee0d081`  
		Last Modified: Fri, 26 Mar 2021 15:03:04 GMT  
		Size: 3.1 MB (3082734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c129b1161496dd5f093240bbcc3a8117babb3970d1b268b5ef2a3b583cf288`  
		Last Modified: Fri, 26 Mar 2021 15:03:19 GMT  
		Size: 130.4 MB (130406650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec06bab51d83666979940922b947a720f6acaca816d2bf3cd332e567591afa4b`  
		Last Modified: Thu, 22 Apr 2021 23:13:03 GMT  
		Size: 14.1 MB (14062057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7f4311425eb37ef28297f5763e749844d439a78264d4863390508759094d6`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1685eb89d16b4bfbe9ff198cfccf641c1de3b8ea23ef56df88b431fed4260572`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 9.6 KB (9557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2045df8ec68a9c233ea9c9dcb3fb5568ea59166bb9912373e550945f7c42c1f`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc56667d904c50234135b3bfefa6630c14e255a6fbd7ee3143d06f8aac839ab9`  
		Last Modified: Thu, 22 Apr 2021 23:12:58 GMT  
		Size: 10.6 KB (10553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5451ef86b75da4eaad3a9248b4b2158b6aca3cb0a19da6c9dfc7a955e8de2038`  
		Last Modified: Thu, 22 Apr 2021 23:12:59 GMT  
		Size: 5.3 MB (5327202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbb2811058d1ddf7c93605f52b4f92cf27c033ae5b026fb74b7584705122c15`  
		Last Modified: Thu, 22 Apr 2021 23:13:48 GMT  
		Size: 213.0 MB (212960397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab321d9643cb04efbdeaff3e7e94f91bd291323f304fc7b2943c5578468939e`  
		Last Modified: Thu, 22 Apr 2021 23:13:26 GMT  
		Size: 953.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edfcc0e4989bb4f0adce15dd3e622084b8b2c6ea9f85223785b1f7bcd097a5d`  
		Last Modified: Thu, 22 Apr 2021 23:13:31 GMT  
		Size: 18.7 MB (18735600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:1813d2e44e1f79784ab44778359fd80a47b37726d4ded32db082ca08eb72f80f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.0 MB (411023034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1109636c471215912302d8affaad06caa663cedee902a569c14ebc0e70e6a9a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:25:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 23 Apr 2021 22:25:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:25:17 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 23 Apr 2021 22:26:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 23 Apr 2021 22:26:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:16:58 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:16:58 GMT
ARG OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:16:59 GMT
ARG EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c
# Fri, 23 Apr 2021 23:17:00 GMT
ARG NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1
# Fri, 23 Apr 2021 23:17:00 GMT
ARG NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096
# Fri, 23 Apr 2021 23:17:01 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.4 org.opencontainers.image.revision=cl210420210407-0944 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 23 Apr 2021 23:17:02 GMT
ENV LIBERTY_VERSION=21.0.0_04
# Fri, 23 Apr 2021 23:17:02 GMT
ARG LIBERTY_URL
# Fri, 23 Apr 2021 23:17:03 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 23 Apr 2021 23:17:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:17:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 23:17:21 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.4 BuildLabel=cl210420210407-0944
# Fri, 23 Apr 2021 23:17:21 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 23 Apr 2021 23:17:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 23 Apr 2021 23:17:24 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Fri, 23 Apr 2021 23:17:25 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 23 Apr 2021 23:17:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 23 Apr 2021 23:17:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=97928b10f7247e2412a5dd78528ae1bd218212eec342f938dec6202a9680616c NON_IBM_SHA=2a518255f7a59a1a003fd0646c8b2424ba655683f8394940a0cad693a7a1fbf1 NOTICES_SHA=d4b0236a5fc49b6308923b87fcd6b4ba4aac33efc02c27f8292c3aa7a532d096 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 23 Apr 2021 23:17:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 23 Apr 2021 23:17:42 GMT
USER 1001
# Fri, 23 Apr 2021 23:17:42 GMT
EXPOSE 9080 9443
# Fri, 23 Apr 2021 23:17:43 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 23 Apr 2021 23:17:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 23 Apr 2021 23:18:44 GMT
ARG VERBOSE=false
# Fri, 23 Apr 2021 23:18:45 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 23 Apr 2021 23:22:46 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 23 Apr 2021 23:23:00 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 23 Apr 2021 23:23:44 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93b87da546ac7aa6705cd2f20bfe70cf04793ac73561e5dd8c579af88754aec`  
		Last Modified: Fri, 23 Apr 2021 22:28:41 GMT  
		Size: 2.7 MB (2676643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268462fc02d2bd9da227784f5f243759923a14cefb3648739ca02e8fa7d63ee7`  
		Last Modified: Fri, 23 Apr 2021 22:28:50 GMT  
		Size: 128.1 MB (128065984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895091e75a5c1ee863c074a41c334973d986bb55cef3d4ba2f8267a2887f8336`  
		Last Modified: Fri, 23 Apr 2021 23:53:50 GMT  
		Size: 14.1 MB (14061390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26d2145efe41abadeb2694f43164f1a155e500e85bf004da26812cd8532de7f`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1dc41aa938b0af86dfd6446147e4484cb5d6bad6e84eb2edb074790b0615a1`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 9.6 KB (9556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0e2666f7e25fefd1dfbbb522189283388626a78a6993958a175bfe3d453daa`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1422da1f78c4ff3f196f908ccd43d884e84e4586193eab1bfe59df39b352b130`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 10.5 KB (10540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a848b971c7539a51ff9771c57f7df448cc5b960c0be0fa5b3c3b547e8589c`  
		Last Modified: Fri, 23 Apr 2021 23:53:47 GMT  
		Size: 5.9 MB (5924580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a29d9ef14335af914d1a4155de231f338e3649b1e962477e8f3c3007227195`  
		Last Modified: Fri, 23 Apr 2021 23:54:16 GMT  
		Size: 213.6 MB (213555213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85098d48d9a85bbbdc1b5f863692bf7b326b94c5f44d091ff39e53fb34a41cc`  
		Last Modified: Fri, 23 Apr 2021 23:54:05 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1e656c995305a66ce28c668c88b221183600d735978d891b72351644e890c2`  
		Last Modified: Fri, 23 Apr 2021 23:54:08 GMT  
		Size: 21.4 MB (21363413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
