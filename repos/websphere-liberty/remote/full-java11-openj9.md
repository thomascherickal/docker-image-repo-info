## `websphere-liberty:full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:5c6456619f9610d19de6b8bcd36e53a27b4b8628007229592ea641cc3f9a6ba2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:49ad5021228ea500c6782f08d64602328151015ff097ca687c003e939b92c516
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.8 MB (317785278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1665f3879bb523f6f34d5586d20b021922e586662dd2c9c21d6239b3876077ba`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:39:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 26 Nov 2020 00:39:43 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:44:57 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Thu, 26 Nov 2020 00:46:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 26 Nov 2020 00:46:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Nov 2020 00:46:47 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 26 Nov 2020 00:48:14 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 26 Nov 2020 00:48:14 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 26 Nov 2020 02:56:55 GMT
ARG VERBOSE=false
# Thu, 26 Nov 2020 02:56:55 GMT
ARG OPENJ9_SCC=true
# Thu, 26 Nov 2020 02:56:55 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Thu, 26 Nov 2020 02:56:56 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Thu, 26 Nov 2020 02:56:56 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Thu, 26 Nov 2020 02:56:56 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 26 Nov 2020 02:56:56 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Thu, 26 Nov 2020 02:56:56 GMT
ARG LIBERTY_URL
# Thu, 26 Nov 2020 02:56:56 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 26 Nov 2020 02:57:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 02:57:07 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Nov 2020 02:57:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Thu, 26 Nov 2020 02:57:07 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 26 Nov 2020 02:57:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 26 Nov 2020 02:57:09 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Thu, 26 Nov 2020 02:57:10 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 26 Nov 2020 02:57:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 26 Nov 2020 02:57:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 26 Nov 2020 02:57:20 GMT
ENV RANDFILE=/tmp/.rnd
# Thu, 26 Nov 2020 02:57:20 GMT
USER 1001
# Thu, 26 Nov 2020 02:57:21 GMT
EXPOSE 9080 9443
# Thu, 26 Nov 2020 02:57:21 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 26 Nov 2020 02:57:21 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 26 Nov 2020 03:01:49 GMT
ARG VERBOSE=false
# Thu, 26 Nov 2020 03:01:49 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 26 Nov 2020 03:04:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 26 Nov 2020 03:04:39 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 26 Nov 2020 03:05:20 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c07f69a5e5c1c84cfd4566011622ffa52b8d00336abda1dd767c51718498628`  
		Last Modified: Thu, 26 Nov 2020 00:56:19 GMT  
		Size: 16.0 MB (16032786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3506268b6e4ebda35c7c28d1d35dd34844cba814fef27e486281e9f71bc12534`  
		Last Modified: Thu, 26 Nov 2020 01:00:01 GMT  
		Size: 42.8 MB (42770641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caf688223f9642bb9f68063d0257e5adcb318bd2c461f7a2cf4484fa84ced29`  
		Last Modified: Thu, 26 Nov 2020 00:59:54 GMT  
		Size: 4.4 MB (4436970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0078a870a54bbf8814a8d6b8ddd47a6dee80cb16b8895843595fb402c57e678b`  
		Last Modified: Thu, 26 Nov 2020 03:10:46 GMT  
		Size: 14.1 MB (14072750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96ef1d3d6c1eeec836c0b71d0113a96e4b2980c6676712f6114d35393d5590`  
		Last Modified: Thu, 26 Nov 2020 03:10:44 GMT  
		Size: 645.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e279cbd3108b4906725a04470574ea9e5be0d480b7d0350ee49b1fb65171364`  
		Last Modified: Thu, 26 Nov 2020 03:10:43 GMT  
		Size: 9.5 KB (9511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ce93e546f7d98529a7a2e44bcc21bc296df77cb119f462af3dab0af74c029c`  
		Last Modified: Thu, 26 Nov 2020 03:10:43 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026d705fbd35934f49e659bfdb932ebb02e4ea0242968f6e4019bac4cff2bf84`  
		Last Modified: Thu, 26 Nov 2020 03:10:44 GMT  
		Size: 10.4 KB (10412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537c5eae0fe52b5d0055872247f1741cd8147267816190740e1b08c7755130bb`  
		Last Modified: Thu, 26 Nov 2020 03:10:44 GMT  
		Size: 2.5 MB (2508416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c719d8c6affde02a53637f61502c0ff778c7b20128f22878d43a22ae8a334`  
		Last Modified: Thu, 26 Nov 2020 03:11:24 GMT  
		Size: 194.6 MB (194612311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d23d4bfbaefe1bd6fe6742a87bffe3372113d567987bbe03ab403aa5164d60b`  
		Last Modified: Thu, 26 Nov 2020 03:11:11 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2703f7ead3952a71ef7b2559ba965797f4f2fed46c432d1e746cfb1a84a319`  
		Last Modified: Thu, 26 Nov 2020 03:11:14 GMT  
		Size: 14.8 MB (14765373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:f1a744cfce0e0dc574f3840fbb76a9a27dfa7b810c038be0afa0f24d730d56f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (322031611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0d8039fef2aff9c5c275ca0ca8b05e31920db2e4510d3288227c21962299a81`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:29:32 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:32:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:32:36 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:32:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:34:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:34:21 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 21 Nov 2020 01:22:18 GMT
ARG VERBOSE=false
# Sat, 21 Nov 2020 01:22:26 GMT
ARG OPENJ9_SCC=true
# Sat, 21 Nov 2020 01:22:39 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Sat, 21 Nov 2020 01:22:53 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Sat, 21 Nov 2020 01:23:01 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Sat, 21 Nov 2020 01:23:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 21 Nov 2020 01:23:14 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Sat, 21 Nov 2020 01:23:20 GMT
ARG LIBERTY_URL
# Sat, 21 Nov 2020 01:23:26 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 21 Nov 2020 01:24:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 21 Nov 2020 01:24:27 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Nov 2020 01:24:32 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Sat, 21 Nov 2020 01:24:37 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 21 Nov 2020 01:24:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 21 Nov 2020 01:24:55 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Sat, 21 Nov 2020 01:24:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 21 Nov 2020 01:25:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 21 Nov 2020 01:25:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 21 Nov 2020 01:26:02 GMT
ENV RANDFILE=/tmp/.rnd
# Sat, 21 Nov 2020 01:26:08 GMT
USER 1001
# Sat, 21 Nov 2020 01:26:13 GMT
EXPOSE 9080 9443
# Sat, 21 Nov 2020 01:26:19 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 21 Nov 2020 01:26:24 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 21 Nov 2020 01:31:43 GMT
ARG VERBOSE=false
# Sat, 21 Nov 2020 01:31:49 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 21 Nov 2020 01:35:44 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Sat, 21 Nov 2020 01:35:46 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 21 Nov 2020 01:37:00 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9518fb573dc23ad650fc0ea068af5f93f07e910761dbb8b83156f14d391027`  
		Last Modified: Wed, 28 Oct 2020 17:53:00 GMT  
		Size: 43.7 MB (43650458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7e2048088ed2d44960340a046c30cd88499c7356ea5d5da70160cb9286e6de`  
		Last Modified: Wed, 28 Oct 2020 17:52:52 GMT  
		Size: 3.5 MB (3464582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751ea3820f34ca6880a0dc2bed79fba1f473fedc7782ec41ffb9290ef2b7bdd`  
		Last Modified: Sat, 21 Nov 2020 01:44:24 GMT  
		Size: 14.1 MB (14073511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80600ba667fcc6ade73c7b8f3591a8d9db43cd19679e7a640f021150c546f67`  
		Last Modified: Sat, 21 Nov 2020 01:44:17 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a48b191116279e4670d23187f30bcef12fc0f129d535db10dabd38e0520eb6`  
		Last Modified: Sat, 21 Nov 2020 01:44:17 GMT  
		Size: 9.5 KB (9548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78876d5e2dff2f98f6ece84b2007ae630c4aa3df48c60f83544ccfc1c3ba9d85`  
		Last Modified: Sat, 21 Nov 2020 01:44:17 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef237db1223acf8724f38b1493dd7150356c2df341b50cdd173ac210b95ae687`  
		Last Modified: Sat, 21 Nov 2020 01:44:18 GMT  
		Size: 10.5 KB (10535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d56de37ee166411188aef327db58aa332876c53b7f503f8ef25aa0a915a6efc`  
		Last Modified: Sat, 21 Nov 2020 01:44:18 GMT  
		Size: 2.4 MB (2402417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52db1b77e5be682d6534ca51d40d84e266205530d9912476d7ff695ee5179899`  
		Last Modified: Sat, 21 Nov 2020 01:45:28 GMT  
		Size: 194.6 MB (194616330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee708a7bfdcfc2af8398ff5d7fa502801280c3de880dab896525f00737571b60`  
		Last Modified: Sat, 21 Nov 2020 01:45:09 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313c4c9baf8ba7fb674a0467c190435757893da2fa3d4d3c355a11b13cf37cc9`  
		Last Modified: Sat, 21 Nov 2020 01:45:13 GMT  
		Size: 13.3 MB (13317472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:ff3800e73c4de13517e5b41657a6cece4e693ef4ce13bbec6fbd8cf01bde8d9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.6 MB (314636314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63407af98887bfb5684a0d2539b966d67c5c2d359723e6b83008f8cfa5d01527`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:47:34 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:49:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:49:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:49:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:51:11 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:51:11 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 21 Nov 2020 01:52:46 GMT
ARG VERBOSE=false
# Sat, 21 Nov 2020 01:52:47 GMT
ARG OPENJ9_SCC=true
# Sat, 21 Nov 2020 01:52:47 GMT
ARG EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95
# Sat, 21 Nov 2020 01:52:48 GMT
ARG NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b
# Sat, 21 Nov 2020 01:52:48 GMT
ARG NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e
# Sat, 21 Nov 2020 01:52:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.12 org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 21 Nov 2020 01:52:50 GMT
ENV LIBERTY_VERSION=20.0.0_12
# Sat, 21 Nov 2020 01:52:50 GMT
ARG LIBERTY_URL
# Sat, 21 Nov 2020 01:52:51 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 21 Nov 2020 01:53:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 21 Nov 2020 01:53:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Nov 2020 01:53:35 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.12 BuildLabel=cl201220201111-0736
# Sat, 21 Nov 2020 01:53:36 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 21 Nov 2020 01:53:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 21 Nov 2020 01:53:41 GMT
COPY dir:87fb88e41281cc95d67404db807cebd05ba85ea3f246dace99de7f445dc641b1 in /opt/ibm/helpers/ 
# Sat, 21 Nov 2020 01:53:42 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 21 Nov 2020 01:53:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 21 Nov 2020 01:53:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=58eed6f817b4ecc5b464f355b0641938c83b95ac22d29b4f657378f887ff4d95 NON_IBM_SHA=454dca0329ea492fc2ddbc03b19031a7eb7a71b45f9e13c89c9fef0f5f51517b NOTICES_SHA=498313e3f283eada744d1fbfd7626473d989d2df58be714f0df0ad561498520e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 21 Nov 2020 01:53:57 GMT
ENV RANDFILE=/tmp/.rnd
# Sat, 21 Nov 2020 01:53:58 GMT
USER 1001
# Sat, 21 Nov 2020 01:53:58 GMT
EXPOSE 9080 9443
# Sat, 21 Nov 2020 01:53:59 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 21 Nov 2020 01:53:59 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 21 Nov 2020 01:59:12 GMT
ARG VERBOSE=false
# Sat, 21 Nov 2020 01:59:12 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 21 Nov 2020 02:03:19 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Sat, 21 Nov 2020 02:03:34 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 21 Nov 2020 02:04:27 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85326a811af266d8284989b860fcf1e92ea12f9c383c5a2b79a622b2096ba7a7`  
		Last Modified: Wed, 28 Oct 2020 18:03:12 GMT  
		Size: 42.0 MB (42029813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426d45bc780f2843a5e6d7b59b2552d62db894ec6a13ee501d17d38dfc0046a1`  
		Last Modified: Wed, 28 Oct 2020 18:03:07 GMT  
		Size: 4.1 MB (4063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13279f8f36f253af9e39bca6baae4422aa2e472afbca893b8cb7ccc04e996e4c`  
		Last Modified: Sat, 21 Nov 2020 02:13:23 GMT  
		Size: 14.1 MB (14072920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118a317992fff68394a957a18dd3405ef697e45ed3e5341d7cf3f5946d7efd41`  
		Last Modified: Sat, 21 Nov 2020 02:12:56 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddf2caaef7d5cad02f8d7d2dce8a26a61f120a58d53b02e23432f42e7687b05`  
		Last Modified: Sat, 21 Nov 2020 02:12:57 GMT  
		Size: 9.5 KB (9544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67049f5f89dcc4806d0b75c013e959568c919f10a3deee89f54f98fcefccbe0b`  
		Last Modified: Sat, 21 Nov 2020 02:12:57 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce42d838bc1a3e97cbad1cf0faa5a2b50633ab224db2247fe51e254c530888ad`  
		Last Modified: Sat, 21 Nov 2020 02:12:56 GMT  
		Size: 10.5 KB (10536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e490413e95f3d1e518fbc8a0bfc355c3900e66324687919450d5422262261902`  
		Last Modified: Sat, 21 Nov 2020 02:13:01 GMT  
		Size: 2.5 MB (2516622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df11248ad7b6dfe5449391f3d63d01bdd8319da57a898dbf0af18e827e29797c`  
		Last Modified: Sat, 21 Nov 2020 02:16:19 GMT  
		Size: 194.6 MB (194616511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5269cd214b4a6d23364b9aba681f8680037826ada695ebbe6a4fd8b8a8d1ba74`  
		Last Modified: Sat, 21 Nov 2020 02:16:14 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416be8e7217950506614f8130b40c8282b79406c00a7935a6e72573ad941c6f7`  
		Last Modified: Sat, 21 Nov 2020 02:16:14 GMT  
		Size: 14.3 MB (14316302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
