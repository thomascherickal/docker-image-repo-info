## `websphere-liberty:full`

```console
$ docker pull websphere-liberty@sha256:114c01b606e245483eca84da2bcc38213749a48316205f7e5993e9d3ff8e1946
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:5c004f535c2a20969a8023a557c0a04c1bc6975baec42027bcd9d184398fb1bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.4 MB (458437876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:633836e24cded908224419ea048a0ae970ddf6175039b331f319e0156ae9229b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 08:40:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 19 Mar 2022 08:41:08 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 08:41:08 GMT
ENV JAVA_VERSION=8.0.7.5
# Sat, 19 Mar 2022 08:41:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Sat, 19 Mar 2022 08:41:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 19 Mar 2022 18:03:39 GMT
ARG VERBOSE=false
# Sat, 19 Mar 2022 18:03:39 GMT
ARG OPENJ9_SCC=true
# Sat, 19 Mar 2022 18:03:39 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Sat, 19 Mar 2022 18:03:39 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Sat, 19 Mar 2022 18:03:39 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Sat, 19 Mar 2022 18:03:39 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 19 Mar 2022 18:03:39 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Sat, 19 Mar 2022 18:03:39 GMT
ARG LIBERTY_URL
# Sat, 19 Mar 2022 18:03:39 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 19 Mar 2022 18:03:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 18:03:51 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 18:03:51 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Sat, 19 Mar 2022 18:03:51 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 19 Mar 2022 18:03:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 19 Mar 2022 18:03:52 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Sat, 19 Mar 2022 18:03:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 19 Mar 2022 18:03:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 19 Mar 2022 18:04:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 19 Mar 2022 18:04:04 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Sat, 19 Mar 2022 18:04:04 GMT
USER 1001
# Sat, 19 Mar 2022 18:04:04 GMT
EXPOSE 9080 9443
# Sat, 19 Mar 2022 18:04:04 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 19 Mar 2022 18:04:04 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 19 Mar 2022 18:04:54 GMT
ARG VERBOSE=false
# Sat, 19 Mar 2022 18:04:54 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 19 Mar 2022 18:08:43 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Sat, 19 Mar 2022 18:08:44 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 19 Mar 2022 18:09:28 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01cc9baeb16a491ae8108620b4a3d924d6c096f56f292cba3c6b4616f628d27`  
		Last Modified: Sat, 19 Mar 2022 08:45:17 GMT  
		Size: 3.0 MB (2959867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccfcd8ba6c9fe56dfa0b24f707ccb58daf68347b133604ade02d18430ec7f52`  
		Last Modified: Sat, 19 Mar 2022 08:45:26 GMT  
		Size: 128.8 MB (128801704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a97579feb9b36e82829ec063edca170baf30b5666889aee38778ee2ef789ac`  
		Last Modified: Sat, 19 Mar 2022 18:24:23 GMT  
		Size: 14.1 MB (14079415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5c307ae06736274004e95586f825db765c2172743c9846aa813f4240ab0f0b`  
		Last Modified: Sat, 19 Mar 2022 18:24:19 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caff7e133ffeaad5342c3c47eee19ac709a18c1eeb265b0be5eb4ee0c4dda66f`  
		Last Modified: Sat, 19 Mar 2022 18:24:18 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671f733fc5fae2547550e18caf50a883ca91437fb93c4bcfbf27782aeb1c4052`  
		Last Modified: Sat, 19 Mar 2022 18:24:19 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9114cf237d36e6f18eaac12883a91fcea2819a040251ffe6c05c1f571ea49e2`  
		Last Modified: Sat, 19 Mar 2022 18:24:18 GMT  
		Size: 10.7 KB (10661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ff172e2f82d8496cfb3e8443b257a41776d87952e9864310d2ed00d1916905`  
		Last Modified: Sat, 19 Mar 2022 18:24:20 GMT  
		Size: 5.7 MB (5716532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707570c95c81242afe3a786d765b49046308e6014b16ce71a7a5943994e170c4`  
		Last Modified: Sat, 19 Mar 2022 18:25:10 GMT  
		Size: 264.0 MB (263979010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ef620cf908c3f6f385ef9e0cb86ba71a5ee347cb35e6936a98b76cbf1ed4f`  
		Last Modified: Sat, 19 Mar 2022 18:24:51 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce114bbf62322019ceee249456e92f16b00037f87fbf3b10c3046145aecbfa47`  
		Last Modified: Sat, 19 Mar 2022 18:24:53 GMT  
		Size: 16.2 MB (16170465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:6e843c46848080a82befcbb6230509adce54f4e4d8f8f28e296896d15c3ab0d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.3 MB (459326302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4818fe2b6efc00bb8c984a6478a486a5a5938aa94a3ce4ea1365b25f1e5f550e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 18 Mar 2022 00:47:57 GMT
ADD file:512f577cb3b73f892801365276edc7835b0fbed63fe39c4e98c86264d363163b in / 
# Fri, 18 Mar 2022 00:48:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:22:29 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 19 Mar 2022 20:23:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:23:04 GMT
ENV JAVA_VERSION=8.0.7.5
# Sat, 19 Mar 2022 20:23:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Sat, 19 Mar 2022 20:24:01 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sun, 20 Mar 2022 01:05:35 GMT
ARG VERBOSE=false
# Sun, 20 Mar 2022 01:05:40 GMT
ARG OPENJ9_SCC=true
# Sun, 20 Mar 2022 01:05:45 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Sun, 20 Mar 2022 01:05:48 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Sun, 20 Mar 2022 01:05:52 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Sun, 20 Mar 2022 01:05:55 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sun, 20 Mar 2022 01:05:58 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Sun, 20 Mar 2022 01:06:03 GMT
ARG LIBERTY_URL
# Sun, 20 Mar 2022 01:06:06 GMT
ARG DOWNLOAD_OPTIONS=
# Sun, 20 Mar 2022 01:07:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 01:07:06 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Mar 2022 01:07:13 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Sun, 20 Mar 2022 01:07:17 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sun, 20 Mar 2022 01:07:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sun, 20 Mar 2022 01:07:45 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Sun, 20 Mar 2022 01:07:47 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sun, 20 Mar 2022 01:08:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sun, 20 Mar 2022 01:08:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sun, 20 Mar 2022 01:08:31 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Sun, 20 Mar 2022 01:08:36 GMT
USER 1001
# Sun, 20 Mar 2022 01:08:40 GMT
EXPOSE 9080 9443
# Sun, 20 Mar 2022 01:08:43 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sun, 20 Mar 2022 01:08:46 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sun, 20 Mar 2022 01:14:04 GMT
ARG VERBOSE=false
# Sun, 20 Mar 2022 01:14:10 GMT
ARG REPOSITORIES_PROPERTIES=
# Sun, 20 Mar 2022 01:18:48 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Sun, 20 Mar 2022 01:18:50 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sun, 20 Mar 2022 01:19:48 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:37a959c2edf986d1489b0000a2dbfecd72195cde6524f2a6545bf3c5d66f6bac`  
		Last Modified: Fri, 18 Mar 2022 00:50:57 GMT  
		Size: 30.4 MB (30438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0903ae718e9dccc2c8f73f39ec1dad40c6cdf53a45f943d30911466db2170a2`  
		Last Modified: Sat, 19 Mar 2022 20:27:10 GMT  
		Size: 3.1 MB (3081922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae49af36e03b0f0572e9db712fca338eaf83bebcaed09b72b8e2988643efb1a`  
		Last Modified: Sat, 19 Mar 2022 20:27:23 GMT  
		Size: 128.3 MB (128315514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9034da9660a8c25d2659bb3ebb54a18bf3043769500e3d46b27a453d71bbc443`  
		Last Modified: Sun, 20 Mar 2022 02:01:49 GMT  
		Size: 14.1 MB (14079822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c61171289533e79ad3fa612e070e004e279ca205d2a37fe0726d185f0233a`  
		Last Modified: Sun, 20 Mar 2022 02:01:43 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf7c8eff0ad3dcbc5a6e7eeb3be15c417edc8cb8844aa6ea1d888d0e5d84b3b`  
		Last Modified: Sun, 20 Mar 2022 02:01:43 GMT  
		Size: 9.7 KB (9679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08770d74b750b8ee395a9c9aaacb54592b6f88c230fb7944ab4697345b42a854`  
		Last Modified: Sun, 20 Mar 2022 02:01:43 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323ba8511085326911913ab1e66c957b78ffda8e1f5a2794c00445be8e8a6556`  
		Last Modified: Sun, 20 Mar 2022 02:01:43 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7134fe9e4a12f3bb6f3a205f3cdb3129c3479542d59ef3613fd957a1dd20f3e3`  
		Last Modified: Sun, 20 Mar 2022 02:01:44 GMT  
		Size: 5.3 MB (5330931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08acfe0359b0d237b56ae31d288d7d7baa5618b78f7c8830b25d6c7a875d277`  
		Last Modified: Sun, 20 Mar 2022 02:02:55 GMT  
		Size: 264.0 MB (263978472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e251100dbf80d14e15b238a23b380d4e812dd8a528d8e193cfcaaeac00de53a`  
		Last Modified: Sun, 20 Mar 2022 02:02:33 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102d99712c1d7abff255b308c37269650a078586529f86d61a519af7c386eb8`  
		Last Modified: Sun, 20 Mar 2022 02:02:36 GMT  
		Size: 14.1 MB (14079313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:4281e9a3f387457ddb0f531658ac6fdad04219bcdcb34bb76e8ded08a74c6322
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **453.7 MB (453653116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ba73a7407cf242f22008c4135f63024c5ed1604e488fa9f27e4830b7c8d0f0`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 18 Mar 2022 00:37:02 GMT
ADD file:ca83c77547f5f41417a9bcad24827780f3cecda3aadc05e3ea075ef651e7a96c in / 
# Fri, 18 Mar 2022 00:37:05 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 17:39:07 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Mar 2022 17:39:13 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 17:39:13 GMT
ENV JAVA_VERSION=8.0.7.5
# Fri, 18 Mar 2022 17:39:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Mar 2022 17:39:56 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 18 Mar 2022 18:20:17 GMT
ARG VERBOSE=false
# Fri, 18 Mar 2022 18:20:17 GMT
ARG OPENJ9_SCC=true
# Fri, 18 Mar 2022 18:20:17 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Fri, 18 Mar 2022 18:20:17 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Fri, 18 Mar 2022 18:20:17 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Fri, 18 Mar 2022 18:20:17 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 18 Mar 2022 18:20:17 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Fri, 18 Mar 2022 18:20:17 GMT
ARG LIBERTY_URL
# Fri, 18 Mar 2022 18:20:18 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 18 Mar 2022 18:20:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 18:20:29 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 18:20:29 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Fri, 18 Mar 2022 18:20:29 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 18 Mar 2022 18:20:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 18 Mar 2022 18:20:30 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Fri, 18 Mar 2022 18:20:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 18 Mar 2022 18:20:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 18 Mar 2022 18:20:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 18 Mar 2022 18:20:38 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 18 Mar 2022 18:20:38 GMT
USER 1001
# Fri, 18 Mar 2022 18:20:38 GMT
EXPOSE 9080 9443
# Fri, 18 Mar 2022 18:20:38 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 18 Mar 2022 18:20:39 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 18 Mar 2022 18:21:41 GMT
ARG VERBOSE=false
# Fri, 18 Mar 2022 18:21:41 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 18 Mar 2022 18:26:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 18 Mar 2022 18:26:07 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 18 Mar 2022 18:26:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:19966aaba2fa737074d039f29b54f413d837daaa9d85f02bc54eddd7d645b73c`  
		Last Modified: Fri, 18 Mar 2022 00:38:33 GMT  
		Size: 25.4 MB (25365461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553aa2187de6f86b870a92100c799a91aeea6cdba4160c02ae3405046344347b`  
		Last Modified: Fri, 18 Mar 2022 17:42:03 GMT  
		Size: 2.7 MB (2676789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d731c8dcad057ee3d07d48519da4b9a1233f150c897e5007a5c745030f03f8b`  
		Last Modified: Fri, 18 Mar 2022 17:42:12 GMT  
		Size: 125.8 MB (125807399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80982480b3e6509bd59b19af241d81c72917da75ebd3df7b1a028a7e6ce1c3a1`  
		Last Modified: Fri, 18 Mar 2022 18:54:26 GMT  
		Size: 14.1 MB (14079419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7405a5463e42b8aa57d81eb3038ae2bff8e6625acc66e8f9140691e4c0330fff`  
		Last Modified: Fri, 18 Mar 2022 18:54:24 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17010258d5909b33a45f957102e28bbf13255b0b4203dd034646f0e045012557`  
		Last Modified: Fri, 18 Mar 2022 18:54:24 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1513319e12c32a623174624b578c1d3b836f787e86c994f0116b0b4e3639a81e`  
		Last Modified: Fri, 18 Mar 2022 18:54:24 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c04830ffe33b1615e8fd11f69ba70786796b81633f68dce1150b083d56c3081`  
		Last Modified: Fri, 18 Mar 2022 18:54:24 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ce6dac5d6046bcfcadefb2bc8b0e7103251b7751c5e139948e60619b78fbf2`  
		Last Modified: Fri, 18 Mar 2022 18:54:25 GMT  
		Size: 5.9 MB (5855057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8540be9b36f101e31de750b243c3987b753ca54b1d725ddaceab2e03622cf100`  
		Last Modified: Fri, 18 Mar 2022 18:54:59 GMT  
		Size: 264.0 MB (263980237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84506e0b453a0005cba5c26dee65959859c0da746fbf2ba63b5b834fa2eee249`  
		Last Modified: Fri, 18 Mar 2022 18:54:47 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f388c9cc63b3717f1c89dffffd078efa9459d839f2883f6a7bee01197eae8cfd`  
		Last Modified: Fri, 18 Mar 2022 18:54:49 GMT  
		Size: 15.9 MB (15866508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
