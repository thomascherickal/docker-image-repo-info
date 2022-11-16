## `websphere-liberty:kernel`

```console
$ docker pull websphere-liberty@sha256:cfdd5b62b0ff15f4521173fae281d64f45bccd8b53f0cae82232ed81636bc21b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:4e9113fd7f10f679efae6e02e12b2599576c720e4241ad3d04ef435fc7ce047f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.1 MB (179133882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db4c3e8434fa16e852cec77ad674ee4a6e30329a9fad11da138aef875782c01a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 16:56:49 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 25 Oct 2022 16:56:58 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 16:56:58 GMT
ENV JAVA_VERSION=8.0.7.16
# Tue, 25 Oct 2022 16:57:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='70b5592485b0188b421cb0a072e913e3f93dfebcbc63096651258b622f19e710';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='2cf9c65de9a8dce78ebb4403b0d83a173cda3b3b5064ce5f6f63236f89e607c0';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='eaae9e57e497ab9850203384a373a473f0d8648b02c1de5c1e01af14794c5af9';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='aa301e7f2fa12ba5b3c2183674d232e8942fd6061ea2efa589d1f404969d810b';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='e091ac9b24b35f1c6cf28f3fb494e3643841bc7949c28bf6899bc384ef547ba7';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 25 Oct 2022 16:57:57 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 26 Oct 2022 19:34:36 GMT
ARG VERBOSE=false
# Wed, 26 Oct 2022 19:34:36 GMT
ARG OPENJ9_SCC=true
# Tue, 15 Nov 2022 03:23:22 GMT
ARG EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0
# Tue, 15 Nov 2022 03:23:22 GMT
ARG NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8
# Tue, 15 Nov 2022 03:23:22 GMT
ARG NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec
# Tue, 15 Nov 2022 03:23:22 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.11 org.opencontainers.image.revision=cl221120221010-1540 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 15 Nov 2022 03:23:22 GMT
ENV LIBERTY_VERSION=22.0.0_11
# Tue, 15 Nov 2022 03:23:22 GMT
ARG LIBERTY_URL
# Tue, 15 Nov 2022 03:23:23 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 15 Nov 2022 03:23:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0 NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8 NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:23:41 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 03:23:41 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.11 BuildLabel=cl221120221010-1540
# Tue, 15 Nov 2022 03:23:41 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 15 Nov 2022 03:23:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0 NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8 NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 15 Nov 2022 03:23:43 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Tue, 15 Nov 2022 03:23:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 15 Nov 2022 03:23:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0 NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8 NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 15 Nov 2022 03:23:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0 NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8 NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 15 Nov 2022 03:23:53 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 15 Nov 2022 03:23:53 GMT
USER 1001
# Tue, 15 Nov 2022 03:23:53 GMT
EXPOSE 9080 9443
# Tue, 15 Nov 2022 03:23:53 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 15 Nov 2022 03:23:53 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c575a748d387bc29aaca33bf9a03ae2a062e61b424be275006c0d73ba2c2273`  
		Last Modified: Tue, 25 Oct 2022 17:00:16 GMT  
		Size: 3.0 MB (2957891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df73c475e4c165c33762ecd295e86b6eb72e5746b0c6badee7693a16b61f040d`  
		Last Modified: Tue, 25 Oct 2022 17:00:25 GMT  
		Size: 129.4 MB (129351634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571ce8ed913bdcb0c1bbdf7729bbcc9be32e9acf7a87fd9bf01a935f800d85e1`  
		Last Modified: Tue, 15 Nov 2022 03:52:37 GMT  
		Size: 14.2 MB (14211250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95d2a19a1004fb04c687e77d860e536b2fb50d6abafb93b8a0dbb0004243ae2`  
		Last Modified: Tue, 15 Nov 2022 03:52:33 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e1f234c117dfd2385dc328983125774857b081a7fab479441dfa1810766b96`  
		Last Modified: Tue, 15 Nov 2022 03:52:34 GMT  
		Size: 9.8 KB (9762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89236850111edd79069ec47942c1ba56f7dacd114d62e12e333b1ada5da603d`  
		Last Modified: Tue, 15 Nov 2022 03:52:34 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61018e6eb697e3a96d82fa25d090b9a27e4658c0875e3096dfc416e9d99443bc`  
		Last Modified: Tue, 15 Nov 2022 03:52:33 GMT  
		Size: 10.7 KB (10747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb66d649467d22bf412ec8e7ffd0d0d2ed8ace150b392bdbf7df18a156ed3252`  
		Last Modified: Tue, 15 Nov 2022 03:52:35 GMT  
		Size: 5.9 MB (5879134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:6fc3432ad61b8c0a2029edfe5d77538d1c2c62a0a39785ed4009867ab282432b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.3 MB (182257109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a31a52d32a8aa59bca6ecfc903493dc0bfc8ac01ee2973463440d604376913d1`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:07:39 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 25 Oct 2022 14:08:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 14:08:09 GMT
ENV JAVA_VERSION=8.0.7.16
# Tue, 25 Oct 2022 14:10:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='70b5592485b0188b421cb0a072e913e3f93dfebcbc63096651258b622f19e710';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='2cf9c65de9a8dce78ebb4403b0d83a173cda3b3b5064ce5f6f63236f89e607c0';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='eaae9e57e497ab9850203384a373a473f0d8648b02c1de5c1e01af14794c5af9';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='aa301e7f2fa12ba5b3c2183674d232e8942fd6061ea2efa589d1f404969d810b';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='e091ac9b24b35f1c6cf28f3fb494e3643841bc7949c28bf6899bc384ef547ba7';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 25 Oct 2022 14:10:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 26 Oct 2022 03:12:54 GMT
ARG VERBOSE=false
# Wed, 26 Oct 2022 03:12:54 GMT
ARG OPENJ9_SCC=true
# Tue, 15 Nov 2022 04:15:13 GMT
ARG EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0
# Tue, 15 Nov 2022 04:15:13 GMT
ARG NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8
# Tue, 15 Nov 2022 04:15:13 GMT
ARG NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec
# Tue, 15 Nov 2022 04:15:14 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.11 org.opencontainers.image.revision=cl221120221010-1540 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 15 Nov 2022 04:15:14 GMT
ENV LIBERTY_VERSION=22.0.0_11
# Tue, 15 Nov 2022 04:15:14 GMT
ARG LIBERTY_URL
# Tue, 15 Nov 2022 04:15:15 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 15 Nov 2022 04:16:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0 NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8 NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:16:04 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 04:16:05 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.11 BuildLabel=cl221120221010-1540
# Tue, 15 Nov 2022 04:16:05 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 15 Nov 2022 04:16:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0 NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8 NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 15 Nov 2022 04:16:08 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Tue, 15 Nov 2022 04:16:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 15 Nov 2022 04:16:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0 NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8 NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 15 Nov 2022 04:16:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0 NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8 NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 15 Nov 2022 04:16:25 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 15 Nov 2022 04:16:26 GMT
USER 1001
# Tue, 15 Nov 2022 04:16:26 GMT
EXPOSE 9080 9443
# Tue, 15 Nov 2022 04:16:26 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 15 Nov 2022 04:16:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3bd07fd743978e6c122138fc96d49720949d9378615ea1610865b23325b7af`  
		Last Modified: Tue, 25 Oct 2022 14:16:02 GMT  
		Size: 3.1 MB (3076044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427cc8d21232d28a4d9cf22428744eede16d9f7648416bbe8a5660da92d3a97f`  
		Last Modified: Tue, 25 Oct 2022 14:16:18 GMT  
		Size: 129.0 MB (129014166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e2f3998405ed64e34685f6ee1feda14a689ed31948b973218a57ea11c52ba9`  
		Last Modified: Tue, 15 Nov 2022 05:13:54 GMT  
		Size: 14.2 MB (14211767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9db5fc37d307cc00c9b8a99c297a0eceec8c321354126bec36e076342f6508a`  
		Last Modified: Tue, 15 Nov 2022 05:13:50 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8d0d4d30a99d58520ac70c3724f8c7e3b3861e0f458d80e42a5e7c38e07f56`  
		Last Modified: Tue, 15 Nov 2022 05:13:50 GMT  
		Size: 9.8 KB (9761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9efd8909d15510643410987caf2a77b822acabff7079844972788749588bef`  
		Last Modified: Tue, 15 Nov 2022 05:13:50 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb32bee6461fb253e2d0fc3296c150b2885695752ee68c2474c6f1bf9701461`  
		Last Modified: Tue, 15 Nov 2022 05:13:50 GMT  
		Size: 10.8 KB (10758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9536903d80c51793fc8d755d73810bd32ae553fa8fc7f2b84de96700e082eab4`  
		Last Modified: Tue, 15 Nov 2022 05:13:52 GMT  
		Size: 5.5 MB (5490419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:7f0fb54da12a204c7a0a69c2003148ab6a089640a26887577d13e0a049e41b69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.8 MB (174781848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7accff557295dce2ab26ee3bcc573802be7cc799108037cc2320d68731b2548`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:02 GMT
ADD file:0843e89b8865a30626cece7a42cf27708a86422aadb28029168b2f159a8768fa in / 
# Tue, 25 Oct 2022 01:23:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:08:47 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 25 Oct 2022 08:09:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 02:13:28 GMT
ENV JAVA_VERSION=8.0.7.20
# Wed, 16 Nov 2022 02:14:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4abf605bdffc703f48c506177ee874da9498a4ee5ef322bfb9b4170b097bf2a8';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='225a8406e9a3134eb8674206caa131a7d5f528de96797a7a0cf69e292465d205';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='052efe7ee98f17af3f027c11b9ef57edd136bf9431b8264a790d48cce905fffd';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='47384a0933d2a60b0126eeb49c44be66124320f70355cd09a238a830906819ff';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='bea07ae6d8d56ad7ae2d4937bed352d39622d364be848a036b111fdf15e50cab';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 16 Nov 2022 02:14:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 16 Nov 2022 02:55:03 GMT
ARG VERBOSE=false
# Wed, 16 Nov 2022 02:55:04 GMT
ARG OPENJ9_SCC=true
# Wed, 16 Nov 2022 02:55:04 GMT
ARG EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0
# Wed, 16 Nov 2022 02:55:04 GMT
ARG NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8
# Wed, 16 Nov 2022 02:55:05 GMT
ARG NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec
# Wed, 16 Nov 2022 02:55:05 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.11 org.opencontainers.image.revision=cl221120221010-1540 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 16 Nov 2022 02:55:06 GMT
ENV LIBERTY_VERSION=22.0.0_11
# Wed, 16 Nov 2022 02:55:06 GMT
ARG LIBERTY_URL
# Wed, 16 Nov 2022 02:55:06 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 16 Nov 2022 02:55:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0 NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8 NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 02:55:29 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 02:55:30 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.11 BuildLabel=cl221120221010-1540
# Wed, 16 Nov 2022 02:55:30 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 16 Nov 2022 02:55:32 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0 NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8 NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 16 Nov 2022 02:55:32 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 16 Nov 2022 02:55:33 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 16 Nov 2022 02:55:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0 NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8 NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 16 Nov 2022 02:55:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ce31500fa2422ed1410137cd50d33e18cf42ad0ae0b5a3e545183ae801869e0 NON_IBM_SHA=1f032aeb46b5f5f4262f123cb2339230e2755cac039cb1bf0285cbb0f37fe7c8 NOTICES_SHA=46056efcb4c0e11e1cc9a33104c4d2ae9b42d566ec74885804914c4eb41ef2ec VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 16 Nov 2022 02:55:46 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 16 Nov 2022 02:55:46 GMT
USER 1001
# Wed, 16 Nov 2022 02:55:47 GMT
EXPOSE 9080 9443
# Wed, 16 Nov 2022 02:55:47 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 16 Nov 2022 02:55:48 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:4cd692a206d359f66e10c4f4f2a37009c4162f022df78a9bb8e8c24def290167`  
		Last Modified: Tue, 25 Oct 2022 01:24:23 GMT  
		Size: 25.4 MB (25371461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b48aa864b900d3e1ae35d49fc6be512e393a95d7020a8372679d9d04253958`  
		Last Modified: Tue, 25 Oct 2022 08:12:34 GMT  
		Size: 2.7 MB (2671897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e9d9054e5f089190a939b775ac219a4fa94f2249aaaded6283a2c2c4e422b`  
		Last Modified: Wed, 16 Nov 2022 02:17:47 GMT  
		Size: 126.5 MB (126472615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc154b271d924345066a7498f50475c78b0cc333ce8ff2dd70dca674f563c6c8`  
		Last Modified: Wed, 16 Nov 2022 03:27:10 GMT  
		Size: 14.2 MB (14211280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82e6ce6c3fd74f25b621f967ca3d461fd1dfef61be6c33b5082f367a983e16f`  
		Last Modified: Wed, 16 Nov 2022 03:27:08 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38e3e85d36e7f31b81852e12f7e306c22ab133578d8fdc8401a0f6beece51c5`  
		Last Modified: Wed, 16 Nov 2022 03:27:08 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ab70c4d36abbae1da8d7908d97aa1153540516f9f2f9b713809f6be38faede`  
		Last Modified: Wed, 16 Nov 2022 03:27:08 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b78a4c43f9dbb7e14161c06f2a0506834cd8d4a2db562ba63a12c904d41b364`  
		Last Modified: Wed, 16 Nov 2022 03:27:08 GMT  
		Size: 10.7 KB (10730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb9f7898fb96f8aebea70db68b9caa6030cab26e223b9094352e48c77a76577`  
		Last Modified: Wed, 16 Nov 2022 03:27:09 GMT  
		Size: 6.0 MB (6033154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
