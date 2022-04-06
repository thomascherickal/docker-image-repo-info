## `websphere-liberty:full`

```console
$ docker pull websphere-liberty@sha256:8de0b824af28b3746a3c6125fedbb83a9280b825b1e923403306e79f722c376f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:cda65fcc714caba7e3c36f5b7435e9bdfc3ac25a35a1d19d6a4131202eb2db7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.4 MB (458358013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5ac205b973d5c45f76f1d8f62de7d9666fa8edc73a87e83caf63db1a09b0df9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:11:03 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 04:11:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:11:10 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 04:11:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 04:11:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:04:50 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:04:50 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:04:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 06:04:50 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 06:04:50 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 06:04:50 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:04:51 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 06:04:51 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:04:51 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:05:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:05:01 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:05:01 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 06:05:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:05:03 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:05:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:05:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:05:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:05:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:05:13 GMT
USER 1001
# Wed, 06 Apr 2022 06:05:14 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:05:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:05:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 06:06:04 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:06:04 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 06:09:55 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 06:09:56 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 06:10:33 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfba7ea970cb1c55200b82df4d841cb3aeceb410b11a8979aa633a92e7d236b`  
		Last Modified: Wed, 06 Apr 2022 04:13:29 GMT  
		Size: 3.0 MB (2959903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7928eec80454bb70ea4d40960304e706827316397e2721ec34143d7e471d489`  
		Last Modified: Wed, 06 Apr 2022 04:13:39 GMT  
		Size: 128.8 MB (128801744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e8321e19197f2773b582a498e2c352f378d117442244e67ab76160b26c151`  
		Last Modified: Wed, 06 Apr 2022 06:34:41 GMT  
		Size: 14.1 MB (14079475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f525ec02b7acf591d7d8eec0bc9312b4d67404d39b2fe6b867cbdd75cda5957`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24de75b5ad0e32a1538636e8cf2db791b896dda43206f4b53cd75447dcdd9d69`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 9.7 KB (9680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17671817a6482e1aab160a13024a37aa3725d833b5e1fe872e40c965b3e60c2`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd49fec10585cc3bbdc3a0fb3580e26135a7b7910e8fef1cc1cded362c8d33c`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5821dc03875268203466d1599daa966b4ca91b58ed9b5391b9d3274d649c7efa`  
		Last Modified: Wed, 06 Apr 2022 06:34:38 GMT  
		Size: 5.7 MB (5698843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c243f60957de1ee44d01c6baaae691fe8078ff83354adf037360a605c61e29f0`  
		Last Modified: Wed, 06 Apr 2022 06:35:23 GMT  
		Size: 264.0 MB (263977874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bea240e7db6ec28462ead5dea5d2b49793e7ca3048380006748d9551ae47aca`  
		Last Modified: Wed, 06 Apr 2022 06:35:09 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf55c107ae9a8dec5f029da6a473b1e6a1de8413e84cbabacf8ee2932c9c6eb5`  
		Last Modified: Wed, 06 Apr 2022 06:35:12 GMT  
		Size: 16.1 MB (16108990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:c97b5678d350c594cbcbd9036c7bb6eb551c40d1fc684f6deba01863d86c196c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.4 MB (459380904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92453735197d834aebbc804122ab90fd2bca3463f14bdd638c9a611e89ee0f6c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:14 GMT
ADD file:1dc494089c70f6414b0a1f5e2e09605266508bf5ec19e1e2fb17028253f8953d in / 
# Wed, 06 Apr 2022 03:35:17 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 05:13:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 05:14:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:14:31 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 05:15:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 05:15:55 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:00:44 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:00:46 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:00:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 11:00:53 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 11:00:56 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 11:00:59 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:01:01 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 11:01:03 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:01:07 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:01:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:01:52 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:01:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 11:02:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:02:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:02:29 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:02:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:02:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:03:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:03:16 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:03:22 GMT
USER 1001
# Wed, 06 Apr 2022 11:03:28 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:03:32 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:03:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 11:12:16 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:12:20 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 11:17:19 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 11:17:36 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 11:19:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:74c6ac89233d470993bd9d67b39dc7ccb63096b55dc274e26eb50345bbecdcd8`  
		Last Modified: Tue, 05 Apr 2022 13:13:08 GMT  
		Size: 30.4 MB (30438429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdbaeb83a31ef16299d247a8ff263c6635af307374780bb9be69adac828283a`  
		Last Modified: Wed, 06 Apr 2022 05:19:24 GMT  
		Size: 3.1 MB (3082224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2b3b642229c677b19f97c99ecf42203b8d144e161b096bac2c2f2423096b3`  
		Last Modified: Wed, 06 Apr 2022 05:19:37 GMT  
		Size: 128.3 MB (128315500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607319fec708d071582f7068356a9b783452155ba745e3ae2a1ee5ff70006816`  
		Last Modified: Wed, 06 Apr 2022 12:00:17 GMT  
		Size: 14.1 MB (14080204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db26f8d06474b6cdae2a54e5b37464ae2d95059cad5bf4f189066796933a20b`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1989f41a81f220c80b3443f5b96a49f0372f9d53626c1551cdb7c72835b58`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3bfd5a575c436bbb31c349cb945f2f841da5996f2fe41fe71c3a5c1c9cc2fd`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96179275284d5d42953fdbb04b7c28b376c018e18dc4e7fa6acadebcd137663a`  
		Last Modified: Wed, 06 Apr 2022 12:00:13 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df489a3f9e1f8998afa4e608455726d81d3a58818050d61fd27c6c7b77244af`  
		Last Modified: Wed, 06 Apr 2022 12:00:13 GMT  
		Size: 5.3 MB (5336752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b042d816e5dae6c615a67e99c9c146f9361cb053c7191a28453ee4bac700dd`  
		Last Modified: Wed, 06 Apr 2022 12:01:20 GMT  
		Size: 264.0 MB (263979859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27a22ff3e3a47f2f395eea6bcdf51b5900894b8bc4088f6bb5a568e5faa585e`  
		Last Modified: Wed, 06 Apr 2022 12:00:57 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395acfb1d10392c0b8bd138f86cd3d941e8ed4e3df73d3dddc2d25c5e1cd20ba`  
		Last Modified: Wed, 06 Apr 2022 12:01:00 GMT  
		Size: 14.1 MB (14125664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:17a16ee52bccd25691b4511b3a476c3b9e8b89db8bb57e2cad48f1a27f1325bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **453.8 MB (453776780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f6c02bef0033fdf780cd7e119e505dd2cc3448e877dacc650f05f9ab493896b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:55 GMT
ADD file:7da6edcff7f600bf3a5d740cd585065c6b3748ff587c0627def91686d1bfe54d in / 
# Tue, 05 Apr 2022 22:41:57 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:04:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 05 Apr 2022 23:04:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:04:27 GMT
ENV JAVA_VERSION=8.0.7.5
# Tue, 05 Apr 2022 23:05:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 05 Apr 2022 23:05:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:21:45 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:21:45 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:21:45 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 00:21:45 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 00:21:45 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 00:21:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:21:46 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 00:21:46 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:21:46 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:22:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:22:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:22:00 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 00:22:01 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:22:03 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:22:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:22:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:22:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:22:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:22:13 GMT
USER 1001
# Wed, 06 Apr 2022 00:22:13 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:22:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:22:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 00:23:26 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:23:27 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 00:28:01 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 00:28:10 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 00:28:39 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:4b0f8a5e4614be4866f08e8772b57664127164f512df03d05a52607176caa02f`  
		Last Modified: Tue, 05 Apr 2022 13:13:37 GMT  
		Size: 25.4 MB (25365860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1df112729db94ceb85cc2f4f1a8a29c4c17240f3414e928932240687367857b`  
		Last Modified: Tue, 05 Apr 2022 23:07:59 GMT  
		Size: 2.7 MB (2676913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7842fa8c2deed61ffe9a36afd3c1544e042b88e440ab57c28e1732e356ea75df`  
		Last Modified: Tue, 05 Apr 2022 23:08:07 GMT  
		Size: 125.8 MB (125807378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404f68c2321c29cbc1068910410523410cf5f547bd14a1a39d22a191b7af2f2c`  
		Last Modified: Wed, 06 Apr 2022 00:59:35 GMT  
		Size: 14.1 MB (14079579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae1055a4b0be252bcf172f8c6844707d527fcef2a35187c9569bef098a77c18`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc478f125deb368d73eb16801b69efb288cb07b229ff40ef29a31cd1fec805c`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 9.7 KB (9682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90d9b68d251175efb44f7e467b8bc09edacfc0fbf0d138d33684cfd78d72d9f`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346a08c2d95ddc678ee0d514318700fdbbc867edbdc372f52a1d50792cf92af`  
		Last Modified: Wed, 06 Apr 2022 00:59:33 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79772bc444250adebe9820159101675bd0b319704a1298e7b58cc96a2fc91830`  
		Last Modified: Wed, 06 Apr 2022 00:59:33 GMT  
		Size: 5.8 MB (5840724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af3906793f5b93df770a0e9c8ab76701e7a7462c459753b23abeb8927f0be8f`  
		Last Modified: Wed, 06 Apr 2022 01:00:07 GMT  
		Size: 264.0 MB (263980552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc4cd25be3f31eced3efee7946ca0b82fb018fd5d8a2ca3ef863f738de062ae`  
		Last Modified: Wed, 06 Apr 2022 00:59:55 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ee76efe1d5ce46952511f6eabd0cc40ccf205b07c26582d2504d6d50a868c`  
		Last Modified: Wed, 06 Apr 2022 00:59:57 GMT  
		Size: 16.0 MB (16003518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
