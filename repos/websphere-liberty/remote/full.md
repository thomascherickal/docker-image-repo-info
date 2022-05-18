## `websphere-liberty:full`

```console
$ docker pull websphere-liberty@sha256:6d1010518a21dfb2d0ec5a3b2f26224c85a78ae6bb735ce4e6992cff2c326d20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:573186249b4f3f751cd9936d3802cbe1969540bfd7bf16ac40b6ae1269f75a60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.8 MB (460812354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6814200bd15a9583c06ee78fe91dc62c622e8f2165bd5bde193e7305d4e75fc3`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:06:17 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 30 Apr 2022 01:06:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:06:25 GMT
ENV JAVA_VERSION=8.0.7.6
# Sat, 30 Apr 2022 01:06:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='04b9e508ec9d206296b4972f1e122a168fc5f2524f7606ec3ade6600cef193a8';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d0fa8483f91717a478d3ae8cca82c8934966a7603287208da0ba6fd2261c544b';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='2532804fa557187bb2b7a57d134b818b5cc9054cc3346d0b6ba93467e337fbdb';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='92323ebeb274e60f48f9301a8fe157382191927e50e97870cd9619461b527b5f';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='62e48b9b65d1266c017a890db6e5b3f24d28e543e04d1cf1ce553b280f9bf2c6';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Sat, 30 Apr 2022 01:06:59 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 30 Apr 2022 05:33:48 GMT
ARG VERBOSE=false
# Sat, 30 Apr 2022 05:33:48 GMT
ARG OPENJ9_SCC=true
# Wed, 18 May 2022 01:11:18 GMT
ARG EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8
# Wed, 18 May 2022 01:11:18 GMT
ARG NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47
# Wed, 18 May 2022 01:11:18 GMT
ARG NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759
# Wed, 18 May 2022 01:11:18 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.5 org.opencontainers.image.revision=cl220520220425-0301 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 18 May 2022 01:11:18 GMT
ENV LIBERTY_VERSION=22.0.0_05
# Wed, 18 May 2022 01:11:18 GMT
ARG LIBERTY_URL
# Wed, 18 May 2022 01:11:18 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 18 May 2022 01:11:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 01:11:33 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 May 2022 01:11:34 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.5 BuildLabel=cl220520220425-0301
# Wed, 18 May 2022 01:11:34 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 18 May 2022 01:11:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 18 May 2022 01:11:35 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 18 May 2022 01:11:35 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 18 May 2022 01:11:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 18 May 2022 01:11:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 18 May 2022 01:11:45 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 18 May 2022 01:11:45 GMT
USER 1001
# Wed, 18 May 2022 01:11:45 GMT
EXPOSE 9080 9443
# Wed, 18 May 2022 01:11:45 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 18 May 2022 01:11:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 18 May 2022 01:12:38 GMT
ARG VERBOSE=false
# Wed, 18 May 2022 01:12:38 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 18 May 2022 01:19:56 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 18 May 2022 01:19:57 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 18 May 2022 01:20:25 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9274cc4ee93edf7c6c542860e9243251f72535f23aa9365dc6f25072d40216`  
		Last Modified: Sat, 30 Apr 2022 01:08:49 GMT  
		Size: 3.0 MB (2959981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f2e31e24dc6a646e66288b5787aba0b0ff58a51a88b9eb0173fe5285690727`  
		Last Modified: Sat, 30 Apr 2022 01:08:58 GMT  
		Size: 129.0 MB (129010262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f8ebe630c95f4f6bd318b3a425bcd91527bd4e3bc6c27871fd7827ef41be28`  
		Last Modified: Wed, 18 May 2022 01:36:21 GMT  
		Size: 14.5 MB (14494270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8939698b73d01ee522f9982536d5dca42e25acdb46737ad985e19d20ac07d813`  
		Last Modified: Wed, 18 May 2022 01:36:17 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2168229f0a6715d3112403c8e2c6b0f742ba337e5db61df51e4a3578e814e9db`  
		Last Modified: Wed, 18 May 2022 01:36:17 GMT  
		Size: 9.7 KB (9681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e2277dea2805c6ec1ef67f76ced41007ab06f21525c0b2d99e3727fddbf5e4`  
		Last Modified: Wed, 18 May 2022 01:36:18 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5731bdf00f6956a7b375374b87943d0158af4d998221a724f4d6c7aade379b09`  
		Last Modified: Wed, 18 May 2022 01:36:17 GMT  
		Size: 10.7 KB (10666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa66e74fe52b89d04d5383806c964ff099df28390c5083e71325ffa0ef8e0d4f`  
		Last Modified: Wed, 18 May 2022 01:36:18 GMT  
		Size: 5.8 MB (5756081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d538d9c9a9980df5638155f34718ad855286a81deff2a12a9a017c4684477d5`  
		Last Modified: Wed, 18 May 2022 01:37:03 GMT  
		Size: 265.6 MB (265553396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d249002a3a1e08ff4a085a0d5aee49eada46942392d17f384cefe1a70323a5a`  
		Last Modified: Wed, 18 May 2022 01:36:49 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1073eb36bcf83008098cf3a30db8882e3191a451c5a13536cddb1f3fe281eab`  
		Last Modified: Wed, 18 May 2022 01:36:52 GMT  
		Size: 16.3 MB (16306991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:3fd43dad9408af87510f4464d805bf0f197b79fff591f478c12c3c55ae8ab9cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.6 MB (460624472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ad086a11dcc1da56accc8e18b3f1ca68e86492909290d5e0becc5afe222e12a`
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
# Sat, 30 Apr 2022 01:50:12 GMT
ENV JAVA_VERSION=8.0.7.6
# Sat, 30 Apr 2022 01:51:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='04b9e508ec9d206296b4972f1e122a168fc5f2524f7606ec3ade6600cef193a8';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d0fa8483f91717a478d3ae8cca82c8934966a7603287208da0ba6fd2261c544b';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='2532804fa557187bb2b7a57d134b818b5cc9054cc3346d0b6ba93467e337fbdb';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='92323ebeb274e60f48f9301a8fe157382191927e50e97870cd9619461b527b5f';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='62e48b9b65d1266c017a890db6e5b3f24d28e543e04d1cf1ce553b280f9bf2c6';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Sat, 30 Apr 2022 01:51:17 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 30 Apr 2022 05:17:10 GMT
ARG VERBOSE=false
# Sat, 30 Apr 2022 05:17:14 GMT
ARG OPENJ9_SCC=true
# Sat, 30 Apr 2022 05:17:15 GMT
ARG EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851
# Sat, 30 Apr 2022 05:17:18 GMT
ARG NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e
# Sat, 30 Apr 2022 05:17:20 GMT
ARG NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024
# Sat, 30 Apr 2022 05:17:22 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.4 org.opencontainers.image.revision=cl220420220328-1303 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 30 Apr 2022 05:17:23 GMT
ENV LIBERTY_VERSION=22.0.0_04
# Sat, 30 Apr 2022 05:17:25 GMT
ARG LIBERTY_URL
# Sat, 30 Apr 2022 05:17:30 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 30 Apr 2022 05:18:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 05:18:04 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Apr 2022 05:18:08 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.4 BuildLabel=cl220420220328-1303
# Sat, 30 Apr 2022 05:18:11 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 30 Apr 2022 05:18:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 30 Apr 2022 05:18:28 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Sat, 30 Apr 2022 05:18:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 30 Apr 2022 05:18:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 30 Apr 2022 05:19:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 30 Apr 2022 05:19:09 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Sat, 30 Apr 2022 05:19:14 GMT
USER 1001
# Sat, 30 Apr 2022 05:19:18 GMT
EXPOSE 9080 9443
# Sat, 30 Apr 2022 05:19:21 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 30 Apr 2022 05:19:26 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 30 Apr 2022 05:24:26 GMT
ARG VERBOSE=false
# Sat, 30 Apr 2022 05:24:29 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 30 Apr 2022 05:29:13 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Sat, 30 Apr 2022 05:29:16 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 30 Apr 2022 05:30:19 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:824dce7232c365d3b1e5b341c057a63216c8b9e75a0fd0729b73ae58d2655cc8`  
		Last Modified: Sat, 30 Apr 2022 01:54:38 GMT  
		Size: 128.5 MB (128516348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b10dc581625e8dcf79edf37edfee120a93bda790ca97d81e2884e61d5ec9ec`  
		Last Modified: Sat, 30 Apr 2022 06:36:47 GMT  
		Size: 14.2 MB (14196654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8dd32b8513f26799b9ad3b6dae1f80343b7c6d1d9671c6f2742a155687b131`  
		Last Modified: Sat, 30 Apr 2022 06:36:38 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ca89cfb601ea754e69e5f9e63564fb2642803b92b69dedc480fd748b36b6c5`  
		Last Modified: Sat, 30 Apr 2022 06:36:38 GMT  
		Size: 9.7 KB (9681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06b05e2564f6109f2fa604cf3ccf6ae8748fe8c5ad84c50c759eccf7f445773`  
		Last Modified: Sat, 30 Apr 2022 06:36:38 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881df693803a824cbd9ad1a7777c845530383e1b92455e3857b69075a0f548a4`  
		Last Modified: Sat, 30 Apr 2022 06:36:38 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e38f204851ad52f51221c02afd3a005c237b674dcb4c3368f9c6ed9be48970f`  
		Last Modified: Sat, 30 Apr 2022 06:36:40 GMT  
		Size: 5.3 MB (5297234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0010ac408966f3ce52ca3e95adc2afb0d95c14007b2b7ca9dd2eecf450da141`  
		Last Modified: Sat, 30 Apr 2022 06:37:55 GMT  
		Size: 265.2 MB (265214718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb47fdcf31b6044d0bc00dcff6d744ccbda1a5f19c7d13ee6d56efd484cc94d0`  
		Last Modified: Sat, 30 Apr 2022 06:37:32 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc98c7b21bed04933a5c6157332302ee5bc26ca25d418789e292da85bb41f684`  
		Last Modified: Sat, 30 Apr 2022 06:37:35 GMT  
		Size: 13.9 MB (13851807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:da1648da9cd6b402387d63441828f661d1fe8a00632daf8582613efde13fa74d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.4 MB (455408408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f747386df299b6e924c0694a4af468b325d843209ee182f48740f5257a21ffd2`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:50 GMT
ADD file:9b5ddd45fc485b5c5ea3d28339d1768fa5d8f60059022a971897d51d94ad5847 in / 
# Fri, 29 Apr 2022 22:49:54 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:27:15 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 29 Apr 2022 23:27:21 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:27:22 GMT
ENV JAVA_VERSION=8.0.7.6
# Fri, 29 Apr 2022 23:28:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='04b9e508ec9d206296b4972f1e122a168fc5f2524f7606ec3ade6600cef193a8';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d0fa8483f91717a478d3ae8cca82c8934966a7603287208da0ba6fd2261c544b';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='2532804fa557187bb2b7a57d134b818b5cc9054cc3346d0b6ba93467e337fbdb';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='92323ebeb274e60f48f9301a8fe157382191927e50e97870cd9619461b527b5f';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='62e48b9b65d1266c017a890db6e5b3f24d28e543e04d1cf1ce553b280f9bf2c6';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 29 Apr 2022 23:28:03 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 30 Apr 2022 01:14:41 GMT
ARG VERBOSE=false
# Sat, 30 Apr 2022 01:14:41 GMT
ARG OPENJ9_SCC=true
# Sat, 30 Apr 2022 01:14:41 GMT
ARG EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851
# Sat, 30 Apr 2022 01:14:42 GMT
ARG NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e
# Sat, 30 Apr 2022 01:14:42 GMT
ARG NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024
# Sat, 30 Apr 2022 01:14:42 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.4 org.opencontainers.image.revision=cl220420220328-1303 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 30 Apr 2022 01:14:43 GMT
ENV LIBERTY_VERSION=22.0.0_04
# Sat, 30 Apr 2022 01:14:43 GMT
ARG LIBERTY_URL
# Sat, 30 Apr 2022 01:14:43 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 30 Apr 2022 01:14:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:14:58 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Apr 2022 01:14:58 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.4 BuildLabel=cl220420220328-1303
# Sat, 30 Apr 2022 01:14:59 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 30 Apr 2022 01:15:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 30 Apr 2022 01:15:01 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Sat, 30 Apr 2022 01:15:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 30 Apr 2022 01:15:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 30 Apr 2022 01:15:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 30 Apr 2022 01:15:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Sat, 30 Apr 2022 01:15:14 GMT
USER 1001
# Sat, 30 Apr 2022 01:15:14 GMT
EXPOSE 9080 9443
# Sat, 30 Apr 2022 01:15:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 30 Apr 2022 01:15:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 30 Apr 2022 01:16:34 GMT
ARG VERBOSE=false
# Sat, 30 Apr 2022 01:16:35 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 30 Apr 2022 01:21:08 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Sat, 30 Apr 2022 01:21:13 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 30 Apr 2022 01:21:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:1347a7b069ceb0e131b6f229b7b96bae189f8e4c594c1933170e278d0ed928b2`  
		Last Modified: Fri, 29 Apr 2022 22:51:49 GMT  
		Size: 25.4 MB (25365828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f94c1c13b8b89cf54909fe9580987f60938a39e09f8c39697300c3a17a3ec1`  
		Last Modified: Fri, 29 Apr 2022 23:30:09 GMT  
		Size: 2.7 MB (2677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06275ac2a17fcdc0af3d5fad5f5da24eb7ecf8a3004379b24dd0062489da9426`  
		Last Modified: Fri, 29 Apr 2022 23:30:17 GMT  
		Size: 126.0 MB (126023446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526431fa9dc5bd7d72595d46b6a45b3ffa7fa1487a9b1cbc98291113a2fe4f43`  
		Last Modified: Sat, 30 Apr 2022 02:07:13 GMT  
		Size: 14.2 MB (14196138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d56570d6faf829d691e509476a0a82fd2727f4c9fad51998666c386a64ba81`  
		Last Modified: Sat, 30 Apr 2022 02:07:11 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc6217d92d87c2e7f9645378f071e35d9baf752fbc5f267dbd679d5d7065dac`  
		Last Modified: Sat, 30 Apr 2022 02:07:11 GMT  
		Size: 9.7 KB (9681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6595126d065352c5e08b2db0e6ab23763266bc8f261c6097537f7abcbc5fefd`  
		Last Modified: Sat, 30 Apr 2022 02:07:11 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3123395afcb24dc24c8c88f0b8481a910de6035d254353c510adbb339e63244b`  
		Last Modified: Sat, 30 Apr 2022 02:07:12 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a388ddf64e692cadd78fee704cda4b11738779305d329d56abf76a3ce58ac4fe`  
		Last Modified: Sat, 30 Apr 2022 02:07:12 GMT  
		Size: 5.9 MB (5901598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c5d187a773be752b6523f41f106f5faf6b26fe5601f525f14fa63378fd939a`  
		Last Modified: Sat, 30 Apr 2022 02:07:43 GMT  
		Size: 265.2 MB (265214801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7702d2096946bb1f97cc533de42665d3e179c6bc98da5e806c0043792f4cab89`  
		Last Modified: Sat, 30 Apr 2022 02:07:32 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7b61aee1dfbf667c522b80ef0b7f3fb4ef1ed2d62781e0d5f67b71033dc33d`  
		Last Modified: Sat, 30 Apr 2022 02:07:34 GMT  
		Size: 16.0 MB (16007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
