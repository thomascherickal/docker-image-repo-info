## `websphere-liberty:kernel`

```console
$ docker pull websphere-liberty@sha256:55e5e3625b43a3b3348a77b5d13bba4538d1f26242e2bcff609128e3b4032bb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:9e51fbd00a4fee3e26889df0b9705180556604b5884d3d7e56d49c37ce672959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178839104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f64657becbbac57727009d229430ce73c7827eb24662951056bfb2950a33867`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:52:33 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 02:52:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:52:40 GMT
ENV JAVA_VERSION=8.0.7.10
# Tue, 07 Jun 2022 02:53:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='5d779014943fa5957ad5dbf2230e99d6a4e1cdc4e8d906414700309a53716a4f';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='607414268c0e2994f21b9c031a81e515286b4689ce283f03a12cc1a5f956fdd3';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='9f1f5b5ae2cf7ecfef9b3a8871e721724cb8edd50b671c557881d5479ecdf5cf';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='1a9d7b060670ee27f8be95e8b781f5c85b4228ae4fe1b33f1daddb5d2e56c926';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c609d711ba6ba2857faa285bb6df225df31d22a387f0857dc08976d0f65e7ba7';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 07 Jun 2022 02:53:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Tue, 07 Jun 2022 07:28:50 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 07:28:50 GMT
ARG OPENJ9_SCC=true
# Mon, 27 Jun 2022 18:31:44 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Mon, 27 Jun 2022 18:31:44 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Mon, 27 Jun 2022 18:31:44 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Mon, 27 Jun 2022 18:31:44 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 27 Jun 2022 18:31:44 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Mon, 27 Jun 2022 18:31:45 GMT
ARG LIBERTY_URL
# Mon, 27 Jun 2022 18:31:45 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 27 Jun 2022 18:32:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jun 2022 18:32:08 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Jun 2022 18:32:08 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Mon, 27 Jun 2022 18:32:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 27 Jun 2022 18:32:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 18:32:10 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 18:32:10 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 18:32:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 18:32:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 18:32:19 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 27 Jun 2022 18:32:19 GMT
USER 1001
# Mon, 27 Jun 2022 18:32:19 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 18:32:19 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 18:32:19 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc337ae35500f1356b4927d94eff4c5c2013592d9465313f05b0e829b69baf`  
		Last Modified: Tue, 07 Jun 2022 02:54:56 GMT  
		Size: 3.0 MB (2960220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4e7d05e1ced7329bd287d158f20ca25e0585e77494a3143adeacc656855fb`  
		Last Modified: Tue, 07 Jun 2022 02:55:06 GMT  
		Size: 129.1 MB (129064174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff3f90a8682454c6257bf9585bf24e2045a8987d4da6f2b7714c55fc4bb02a0`  
		Last Modified: Mon, 27 Jun 2022 19:32:46 GMT  
		Size: 14.4 MB (14394423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463a05703c58e1ef0a2b576d1664d42bb3e0d0668a49ecff9537e505ba62dd86`  
		Last Modified: Mon, 27 Jun 2022 19:32:42 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489042badc4d96832a548c6c77a89a21ba8855cc7a3be5621b37c991ebe7270f`  
		Last Modified: Mon, 27 Jun 2022 19:32:42 GMT  
		Size: 9.8 KB (9755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e049c43a9a65f6f083d614f3c6fb25af942afb0750c5234c90be93b694c4f4fd`  
		Last Modified: Mon, 27 Jun 2022 19:32:42 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50328adb5f51ac79bb8f2ce8902b6553f113ad35bd8900832cd59d28b430984e`  
		Last Modified: Mon, 27 Jun 2022 19:32:42 GMT  
		Size: 10.7 KB (10728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3f9f20707dd143bf7e117947ecbc4e4ab945d9cb0dad3e53148f2fa9e3f48`  
		Last Modified: Mon, 27 Jun 2022 19:32:44 GMT  
		Size: 5.7 MB (5687208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:c1b9411be3c50dcc165b4a463196ec3b8b8d92ccc9bfdbcea757423df1d10c95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.9 MB (181937370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c796e3e0574928199e4e030b14a3e4663b98a86ac9e576cbcae70c8281a98215`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:00 GMT
ADD file:2d91cfcbab5facf9c027064efd477cfde81eca0c1a62c6611ac694bafb94d817 in / 
# Fri, 29 Apr 2022 23:22:04 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:49:39 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 30 Apr 2022 01:50:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Jun 2022 18:17:09 GMT
ENV JAVA_VERSION=8.0.7.10
# Wed, 01 Jun 2022 18:18:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='5d779014943fa5957ad5dbf2230e99d6a4e1cdc4e8d906414700309a53716a4f';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='607414268c0e2994f21b9c031a81e515286b4689ce283f03a12cc1a5f956fdd3';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='9f1f5b5ae2cf7ecfef9b3a8871e721724cb8edd50b671c557881d5479ecdf5cf';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='1a9d7b060670ee27f8be95e8b781f5c85b4228ae4fe1b33f1daddb5d2e56c926';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c609d711ba6ba2857faa285bb6df225df31d22a387f0857dc08976d0f65e7ba7';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 01 Jun 2022 18:18:20 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 01 Jun 2022 18:48:57 GMT
ARG VERBOSE=false
# Wed, 01 Jun 2022 18:48:59 GMT
ARG OPENJ9_SCC=true
# Wed, 01 Jun 2022 18:49:05 GMT
ARG EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8
# Wed, 01 Jun 2022 18:49:11 GMT
ARG NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47
# Wed, 01 Jun 2022 18:49:17 GMT
ARG NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759
# Wed, 01 Jun 2022 18:49:21 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.5 org.opencontainers.image.revision=cl220520220425-0301 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 01 Jun 2022 18:49:27 GMT
ENV LIBERTY_VERSION=22.0.0_05
# Wed, 01 Jun 2022 18:49:36 GMT
ARG LIBERTY_URL
# Wed, 01 Jun 2022 18:49:47 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 01 Jun 2022 18:50:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Jun 2022 18:50:33 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 18:50:36 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.5 BuildLabel=cl220520220425-0301
# Wed, 01 Jun 2022 18:50:39 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 01 Jun 2022 18:50:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 01 Jun 2022 18:50:51 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 01 Jun 2022 18:50:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 01 Jun 2022 18:50:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 01 Jun 2022 18:51:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 01 Jun 2022 18:51:23 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 01 Jun 2022 18:51:26 GMT
USER 1001
# Wed, 01 Jun 2022 18:51:28 GMT
EXPOSE 9080 9443
# Wed, 01 Jun 2022 18:51:31 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 01 Jun 2022 18:51:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:c70b79613e1f9e69f0d6473fa0b3f8b10d376e24350617c381ed64978f4bae97`  
		Last Modified: Fri, 29 Apr 2022 23:24:58 GMT  
		Size: 30.4 MB (30443183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b9fc7dc4c2bad9d9f7db0ffd5b499212f90be1d458552dba4bd7e526ede046`  
		Last Modified: Sat, 30 Apr 2022 01:54:24 GMT  
		Size: 3.1 MB (3082255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ff7a5c271ccdc1d007ed16e12fb41d0725701884213399a686c9417d433a53`  
		Last Modified: Wed, 01 Jun 2022 18:21:30 GMT  
		Size: 128.6 MB (128583169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e24227bb0fecd05ab41f61d2216aa24004916dfbb16bc3dacddd5d8ee8e9c66`  
		Last Modified: Wed, 01 Jun 2022 19:29:25 GMT  
		Size: 14.5 MB (14514714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a9cd5f95e26818c13e6ac235e73df5072880c5491eb9726c2459ae1f773cd`  
		Last Modified: Wed, 01 Jun 2022 19:29:19 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19043b34080cc2ac12091b6b765c716c3c2bb18a7c7aa0377fed485dd10316c5`  
		Last Modified: Wed, 01 Jun 2022 19:29:19 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58acefc319da94c8afdd745cf05d90e8c1e237d3a866a685c0f67294d6ab9535`  
		Last Modified: Wed, 01 Jun 2022 19:29:19 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a17477ff2baa5e8df3c225f0ca99e77ba6cfc142cbf943a608465e0ed99bfd3`  
		Last Modified: Wed, 01 Jun 2022 19:29:19 GMT  
		Size: 10.7 KB (10665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f521b4ca8971c5b8ba01e95f073a4d42150c4d0e31132c7a34a9b86271b93e3`  
		Last Modified: Wed, 01 Jun 2022 19:29:20 GMT  
		Size: 5.3 MB (5292734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:e522ee6df5320bc00b36a4782a026c1eec77e4cae7c4fed5c80fcfec31310f2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.4 MB (174385081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c28c2f4f357b483c7e2619fd7d23dd2962caf393428389d94fd2d3107750a729`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 04:04:44 GMT
ADD file:e2caa30d22701eeadebe1abd66923745f75d170d7baa51a62119576c31b7f89c in / 
# Tue, 07 Jun 2022 04:04:47 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:27:04 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 06:27:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:27:24 GMT
ENV JAVA_VERSION=8.0.7.10
# Tue, 07 Jun 2022 06:28:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='5d779014943fa5957ad5dbf2230e99d6a4e1cdc4e8d906414700309a53716a4f';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='607414268c0e2994f21b9c031a81e515286b4689ce283f03a12cc1a5f956fdd3';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='9f1f5b5ae2cf7ecfef9b3a8871e721724cb8edd50b671c557881d5479ecdf5cf';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='1a9d7b060670ee27f8be95e8b781f5c85b4228ae4fe1b33f1daddb5d2e56c926';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c609d711ba6ba2857faa285bb6df225df31d22a387f0857dc08976d0f65e7ba7';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 07 Jun 2022 06:28:32 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Tue, 07 Jun 2022 08:03:31 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 08:03:32 GMT
ARG OPENJ9_SCC=true
# Mon, 27 Jun 2022 17:56:00 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Mon, 27 Jun 2022 17:56:00 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Mon, 27 Jun 2022 17:56:00 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Mon, 27 Jun 2022 17:56:00 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 27 Jun 2022 17:56:00 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Mon, 27 Jun 2022 17:56:01 GMT
ARG LIBERTY_URL
# Mon, 27 Jun 2022 17:56:01 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 27 Jun 2022 17:56:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jun 2022 17:56:14 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Jun 2022 17:56:14 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Mon, 27 Jun 2022 17:56:14 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 27 Jun 2022 17:56:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 17:56:16 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 17:56:16 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 17:56:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 17:56:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 17:56:24 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 27 Jun 2022 17:56:24 GMT
USER 1001
# Mon, 27 Jun 2022 17:56:25 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 17:56:25 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 17:56:25 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:048a87c6fcb9ea8de843bbbe647d14716098af0741f7f59e30c60f39b96b4397`  
		Last Modified: Tue, 07 Jun 2022 04:07:30 GMT  
		Size: 25.4 MB (25370236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c178b02e888a022df784ee042a75ea8e48f1db295aec033725e7e6edc51cc1ca`  
		Last Modified: Tue, 07 Jun 2022 06:31:44 GMT  
		Size: 2.7 MB (2677363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac1fe4af5f33477aea620c2c44c3756da1ddd6f89605a5f6e20fbd8accca03f`  
		Last Modified: Tue, 07 Jun 2022 06:31:53 GMT  
		Size: 126.1 MB (126076451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37f890559078c0134c992b6817517e53a38c91dc4d9250e8b57177131ac4c8e`  
		Last Modified: Mon, 27 Jun 2022 18:50:31 GMT  
		Size: 14.4 MB (14398488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09b08e6f4ee0b9c12a11b52d72f0dea77fe2cd01efe4733876441550e661b56`  
		Last Modified: Mon, 27 Jun 2022 18:50:29 GMT  
		Size: 709.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1156c3bf7800a62d696ec43d365c3be16236c6f2a3d79f5ef18b7345c1e2a7a`  
		Last Modified: Mon, 27 Jun 2022 18:50:29 GMT  
		Size: 9.8 KB (9754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe580b8ca0e92eb94205c58eb52bea1751c10d290657990f2762cb6f6c20b0f1`  
		Last Modified: Mon, 27 Jun 2022 18:50:29 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2019191db1cad05a1c84c4c97ff60eb0dd78d5282da2171aede57e075da9fa0d`  
		Last Modified: Mon, 27 Jun 2022 18:50:29 GMT  
		Size: 10.7 KB (10749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b26d408dd71b1e69f3852aa92b75659e5dc319ddf508bf0b1607ba9ba5f88`  
		Last Modified: Mon, 27 Jun 2022 18:50:30 GMT  
		Size: 5.8 MB (5841055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
