## `websphere-liberty:full`

```console
$ docker pull websphere-liberty@sha256:246351e4976ccce1be52fd9e43b0c2590d2ad892761fc18b5efe954b5758465f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:5b5db5260ce6b5a2b4e95adc44653492ab721baf249c7540bb6b259eb0d74f0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.6 MB (476612329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ced08ddcf579730570a6ac9043f757c854843c87bb7b84905b7fc2afc8ef8c07`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 17:13:23 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 05 Oct 2022 17:13:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:13:31 GMT
ENV JAVA_VERSION=8.0.7.16
# Wed, 05 Oct 2022 17:14:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='70b5592485b0188b421cb0a072e913e3f93dfebcbc63096651258b622f19e710';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='2cf9c65de9a8dce78ebb4403b0d83a173cda3b3b5064ce5f6f63236f89e607c0';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='eaae9e57e497ab9850203384a373a473f0d8648b02c1de5c1e01af14794c5af9';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='aa301e7f2fa12ba5b3c2183674d232e8942fd6061ea2efa589d1f404969d810b';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='e091ac9b24b35f1c6cf28f3fb494e3643841bc7949c28bf6899bc384ef547ba7';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 05 Oct 2022 17:14:24 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 06 Oct 2022 07:23:04 GMT
ARG VERBOSE=false
# Thu, 06 Oct 2022 07:23:04 GMT
ARG OPENJ9_SCC=true
# Thu, 06 Oct 2022 07:23:04 GMT
ARG EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb
# Thu, 06 Oct 2022 07:23:05 GMT
ARG NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34
# Thu, 06 Oct 2022 07:23:05 GMT
ARG NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725
# Thu, 06 Oct 2022 07:23:05 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.10 org.opencontainers.image.revision=cl221020220912-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 06 Oct 2022 07:23:05 GMT
ENV LIBERTY_VERSION=22.0.0_10
# Thu, 06 Oct 2022 07:23:05 GMT
ARG LIBERTY_URL
# Thu, 06 Oct 2022 07:23:05 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 06 Oct 2022 07:23:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34 NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 07:23:23 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 07:23:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.10 BuildLabel=cl221020220912-1100
# Thu, 06 Oct 2022 07:23:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 06 Oct 2022 07:23:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34 NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 06 Oct 2022 07:23:25 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Thu, 06 Oct 2022 07:23:25 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 06 Oct 2022 07:23:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34 NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 06 Oct 2022 07:23:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34 NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 06 Oct 2022 07:23:35 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 06 Oct 2022 07:23:35 GMT
USER 1001
# Thu, 06 Oct 2022 07:23:35 GMT
EXPOSE 9080 9443
# Thu, 06 Oct 2022 07:23:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 06 Oct 2022 07:23:35 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 06 Oct 2022 07:24:34 GMT
ARG VERBOSE=false
# Thu, 06 Oct 2022 07:24:34 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 06 Oct 2022 07:31:39 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 06 Oct 2022 07:31:40 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 06 Oct 2022 07:32:10 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9d8b98df188102d0298ec847e22cee30b83e6a2203144208de17a84f4e915a`  
		Last Modified: Wed, 05 Oct 2022 17:16:34 GMT  
		Size: 3.0 MB (2957821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8aaac34b6dd2dba7f754f536437814e87bcffe5ab4a0f84ce6c4f14269eb152`  
		Last Modified: Wed, 05 Oct 2022 17:16:43 GMT  
		Size: 129.4 MB (129351639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7845abd95e19803e0ff89699bc8570266fd48eb6dd56d4c73bc71e46b99750`  
		Last Modified: Thu, 06 Oct 2022 08:38:50 GMT  
		Size: 14.2 MB (14178597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5502fe36f77c399275201fe623c521ac9afee48cb59282b80bae516e0741b2ff`  
		Last Modified: Thu, 06 Oct 2022 08:38:46 GMT  
		Size: 681.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb527506fedb71245e4b787570e88141f8045a8081b9d26d724aa2ad18787bc1`  
		Last Modified: Thu, 06 Oct 2022 08:38:46 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324d453babf44de3070ba3ad7bc0f578f7e26877c88c3ab6ca76c73c09280f43`  
		Last Modified: Thu, 06 Oct 2022 08:38:46 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a72aad74c3388779b3dc76d376ba12e938370a660eab262333a6c853bf271c`  
		Last Modified: Thu, 06 Oct 2022 08:38:46 GMT  
		Size: 10.7 KB (10735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7065d8b0e2d19d83ff2e885268d5beb207866734c9123b0e3b63bc74b4601e`  
		Last Modified: Thu, 06 Oct 2022 08:38:47 GMT  
		Size: 5.8 MB (5781542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7b8e3c635cc36ec4940218763695810b384ea0203c1e6b3f70a161042e0114`  
		Last Modified: Thu, 06 Oct 2022 08:39:36 GMT  
		Size: 281.6 MB (281600255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeed219eb45131cc5568a600d9d228caae972373785e88e74d3951d5dc3ac7a2`  
		Last Modified: Thu, 06 Oct 2022 08:39:22 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af35391d1adc04f112d8488ec14d4c569cf0e85075e34b696963ad5d3fdf09fd`  
		Last Modified: Thu, 06 Oct 2022 08:39:25 GMT  
		Size: 16.0 MB (16008229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:6603891984f8f4031d42a9f43acc8dabf901dfce2b0d50da2252a37354c78c22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **477.7 MB (477661808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea0444156990fd584b9ec5b0068a9850c4d780064e5185245521dc4679c6441`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 05 Oct 2022 10:51:52 GMT
ADD file:d93b8e74342ae6048a42c90c30192dd384e92b697ad4d8d5944868e03325820c in / 
# Wed, 05 Oct 2022 10:51:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 20:30:38 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 05 Oct 2022 20:30:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 20:30:56 GMT
ENV JAVA_VERSION=8.0.7.16
# Wed, 05 Oct 2022 20:33:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='70b5592485b0188b421cb0a072e913e3f93dfebcbc63096651258b622f19e710';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='2cf9c65de9a8dce78ebb4403b0d83a173cda3b3b5064ce5f6f63236f89e607c0';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='eaae9e57e497ab9850203384a373a473f0d8648b02c1de5c1e01af14794c5af9';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='aa301e7f2fa12ba5b3c2183674d232e8942fd6061ea2efa589d1f404969d810b';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='e091ac9b24b35f1c6cf28f3fb494e3643841bc7949c28bf6899bc384ef547ba7';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 05 Oct 2022 20:33:17 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 05 Oct 2022 22:34:11 GMT
ARG VERBOSE=false
# Wed, 05 Oct 2022 22:34:12 GMT
ARG OPENJ9_SCC=true
# Wed, 05 Oct 2022 22:34:12 GMT
ARG EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb
# Wed, 05 Oct 2022 22:34:13 GMT
ARG NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34
# Wed, 05 Oct 2022 22:34:13 GMT
ARG NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725
# Wed, 05 Oct 2022 22:34:13 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.10 org.opencontainers.image.revision=cl221020220912-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 05 Oct 2022 22:34:14 GMT
ENV LIBERTY_VERSION=22.0.0_10
# Wed, 05 Oct 2022 22:34:14 GMT
ARG LIBERTY_URL
# Wed, 05 Oct 2022 22:34:14 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 05 Oct 2022 22:34:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34 NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 22:34:55 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 22:34:55 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.10 BuildLabel=cl221020220912-1100
# Wed, 05 Oct 2022 22:34:55 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 05 Oct 2022 22:34:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34 NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 05 Oct 2022 22:34:58 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 05 Oct 2022 22:34:59 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 05 Oct 2022 22:35:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34 NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 05 Oct 2022 22:35:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34 NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 05 Oct 2022 22:35:15 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 05 Oct 2022 22:35:15 GMT
USER 1001
# Wed, 05 Oct 2022 22:35:16 GMT
EXPOSE 9080 9443
# Wed, 05 Oct 2022 22:35:16 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 05 Oct 2022 22:35:17 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 05 Oct 2022 22:37:59 GMT
ARG VERBOSE=false
# Wed, 05 Oct 2022 22:37:59 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 05 Oct 2022 22:51:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 05 Oct 2022 22:51:43 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 05 Oct 2022 22:52:35 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:faece833463c99bd10748da29171f2d588a627912f7bbb982b3ca4512dd39eed`  
		Last Modified: Wed, 05 Oct 2022 10:54:03 GMT  
		Size: 30.4 MB (30442565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52af0b72f683bca4c76215658777957eba73fde39f2157d70f361b51f1e4c42`  
		Last Modified: Wed, 05 Oct 2022 20:38:46 GMT  
		Size: 3.1 MB (3075970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46038b192d2e7c544903b03f01644aad2ba1b5d0e70be5a02dac1b3997ff4bd`  
		Last Modified: Wed, 05 Oct 2022 20:39:02 GMT  
		Size: 129.0 MB (129014178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df214124ef3129c9d23e801433511dc9523afaecc76ead85623f8293d5761f5d`  
		Last Modified: Thu, 06 Oct 2022 01:00:44 GMT  
		Size: 14.2 MB (14179054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dad937f24561e59f398a1fa1912ded0549cf466931f6269d56e1d602a850a6`  
		Last Modified: Thu, 06 Oct 2022 01:00:39 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b2e9ede0732dde4300a47b1d39fadbcc5970c466fb76a87aa4b97bdd606d6`  
		Last Modified: Thu, 06 Oct 2022 01:00:39 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40047f82754a673adde51b41e5f8f0d597f7f905298d176332dd4988ee0b4564`  
		Last Modified: Thu, 06 Oct 2022 01:00:39 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfdd39276a4b6a129d8610e4c0a79f6fe9b40f9a6e28958d1cde7aef6176865`  
		Last Modified: Thu, 06 Oct 2022 01:00:39 GMT  
		Size: 10.7 KB (10740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d61cfac976e78b8e821694cc79d5b9a9d6be8d8203c8b16b0707b96b9bde6`  
		Last Modified: Thu, 06 Oct 2022 01:00:40 GMT  
		Size: 5.5 MB (5478312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f52e7ac65351b2b23fb7e4629b53c27729413b322f832825e01bcd57cd5cfaa`  
		Last Modified: Thu, 06 Oct 2022 01:01:43 GMT  
		Size: 281.6 MB (281601177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2026ac92d291fe717e6b17e6cab1285a29e06b060043d209037947fe1b6002d`  
		Last Modified: Thu, 06 Oct 2022 01:01:17 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5facfbdb92df406d42190a868c77bb03b67a7d976dc61451602775e7366e11c`  
		Last Modified: Thu, 06 Oct 2022 01:01:21 GMT  
		Size: 13.8 MB (13848153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:3325a06aadbb3ff26fe06bcc23288626d2d2ac3875eb0d4745f96627f6f7076a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **472.3 MB (472293222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08c58e419f1cb8c5578699147e5b229dff64b3cae11d438aa4d65df219e6a7c5`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 04 Oct 2022 23:52:31 GMT
ADD file:29c2a2a72a634a5f21c2f37cfd38da282528b75f75124d04e56a2f86f2e64121 in / 
# Tue, 04 Oct 2022 23:52:34 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:07:07 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 05 Oct 2022 08:07:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:07:26 GMT
ENV JAVA_VERSION=8.0.7.16
# Wed, 05 Oct 2022 08:08:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='70b5592485b0188b421cb0a072e913e3f93dfebcbc63096651258b622f19e710';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='2cf9c65de9a8dce78ebb4403b0d83a173cda3b3b5064ce5f6f63236f89e607c0';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='eaae9e57e497ab9850203384a373a473f0d8648b02c1de5c1e01af14794c5af9';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='aa301e7f2fa12ba5b3c2183674d232e8942fd6061ea2efa589d1f404969d810b';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='e091ac9b24b35f1c6cf28f3fb494e3643841bc7949c28bf6899bc384ef547ba7';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 05 Oct 2022 08:08:33 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 05 Oct 2022 16:19:39 GMT
ARG VERBOSE=false
# Wed, 05 Oct 2022 16:19:39 GMT
ARG OPENJ9_SCC=true
# Wed, 05 Oct 2022 16:19:39 GMT
ARG EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb
# Wed, 05 Oct 2022 16:19:39 GMT
ARG NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34
# Wed, 05 Oct 2022 16:19:39 GMT
ARG NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725
# Wed, 05 Oct 2022 16:19:40 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.10 org.opencontainers.image.revision=cl221020220912-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 05 Oct 2022 16:19:40 GMT
ENV LIBERTY_VERSION=22.0.0_10
# Wed, 05 Oct 2022 16:19:40 GMT
ARG LIBERTY_URL
# Wed, 05 Oct 2022 16:19:40 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 05 Oct 2022 16:19:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34 NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:19:57 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:19:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.10 BuildLabel=cl221020220912-1100
# Wed, 05 Oct 2022 16:19:57 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 05 Oct 2022 16:19:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34 NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 05 Oct 2022 16:19:59 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 05 Oct 2022 16:19:59 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 05 Oct 2022 16:20:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34 NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 05 Oct 2022 16:20:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=44a2cb9704f0ed8e871e9d1a8faa55563d093d0c34af3c248492dd1790a794eb NON_IBM_SHA=9e1ddbc876eb5fd3182799b2ccf6619f23acfe6d4b0b8ee82c72e3944ad15b34 NOTICES_SHA=1f852693234e6b9fabccb4218a21a88b485300dccd76ee089fb007aaf3180725 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 05 Oct 2022 16:20:08 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 05 Oct 2022 16:20:08 GMT
USER 1001
# Wed, 05 Oct 2022 16:20:08 GMT
EXPOSE 9080 9443
# Wed, 05 Oct 2022 16:20:08 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 05 Oct 2022 16:20:09 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 05 Oct 2022 16:21:13 GMT
ARG VERBOSE=false
# Wed, 05 Oct 2022 16:21:13 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 05 Oct 2022 16:27:58 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 05 Oct 2022 16:28:07 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 05 Oct 2022 16:28:32 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:f41c9e2df5b8fcd28b58de30866b751466a2cbad7eb8f43e02d799439fb377cf`  
		Last Modified: Tue, 04 Oct 2022 23:54:09 GMT  
		Size: 25.4 MB (25370644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42b030bfbe7d3d22ba17686023d66542eece08a7b4916da1aa44dbd0fdc84f3`  
		Last Modified: Wed, 05 Oct 2022 08:11:26 GMT  
		Size: 2.7 MB (2671847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078467334fda3076e58e9a437af8f5303db9291ca36790c92b7b884fa6d89fba`  
		Last Modified: Wed, 05 Oct 2022 08:11:35 GMT  
		Size: 126.5 MB (126472218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98037cd0db6f44155f2ff26796c0c26797d053fe9af056b1589035fa38d4e11e`  
		Last Modified: Wed, 05 Oct 2022 17:34:10 GMT  
		Size: 14.2 MB (14178626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5caf01c97d3711ccb3e5639ba2cbffde71a3098e50702c99bbd50011bfc69264`  
		Last Modified: Wed, 05 Oct 2022 17:34:08 GMT  
		Size: 677.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac26e60a6e24301d8ba60e363c84d1057203400d9ef95352f2d1d973d298455`  
		Last Modified: Wed, 05 Oct 2022 17:34:08 GMT  
		Size: 9.8 KB (9759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3851becf74822c2028f61598a62f77e896e445a3b1c6171d789930919bebf7`  
		Last Modified: Wed, 05 Oct 2022 17:34:08 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4a90af2fcc7385ddb569c25a32240c267df8400af1b6d4cb73d025634d985a`  
		Last Modified: Wed, 05 Oct 2022 17:34:08 GMT  
		Size: 10.7 KB (10735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a57437e3920326925397b3a3bc10cdcc67a2a3288842c7160e2676fe4b7015`  
		Last Modified: Wed, 05 Oct 2022 17:34:09 GMT  
		Size: 6.0 MB (6004294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d198fbf0536f35b6d1dabeb35fbdc9f413663ae9e71ca3ea1ebe69a041974fb`  
		Last Modified: Wed, 05 Oct 2022 17:34:43 GMT  
		Size: 281.6 MB (281600638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ebbac8e539c6e01d6816436fba62f2750c67a1282c8fa880c1ce47c42869bc`  
		Last Modified: Wed, 05 Oct 2022 17:34:31 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b6fdd7ac142565671c047fd0617e62ae6d16de5509ca9765597d0866fd8935`  
		Last Modified: Wed, 05 Oct 2022 17:34:33 GMT  
		Size: 16.0 MB (15972565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
