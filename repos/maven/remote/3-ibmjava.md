## `maven:3-ibmjava`

```console
$ docker pull maven@sha256:3963c1cfb1218357c5900093f8873020c388ad9e4955dd4f23d0fcef3b59bb53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-ibmjava` - linux; amd64

```console
$ docker pull maven@sha256:4ea0243ee765a8d4cbaa585cc092a1328a6ca5f1dbd4e6efb18437d09f5e700b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (234996856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0798698a11e976bb4de325d824ef818152865ae5c14c24844fd3c4f243b903e`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:55:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:55:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:55:32 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:57:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='953586dcb1870406d51fc0f346e2be062471d7dc67dce21ba2009cff0a46724f';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='09705ba9b6c53105062fd7764f9a066bfe5e2f58a64662d29c1eb030d51252e1';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e233b23f00ecda6a8e8fffe4b7c0675c3574754d300b680e70f423a60d047874';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e81cde52da8dd39160a70c98453e379f1286bb39e58f01ba94a63e45e31e2d34';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='dfc67c2861e00265140287091a713496840f5793946e087825f96c7afd4a8a50';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:57:31 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Tue, 23 Nov 2021 01:04:29 GMT
ARG MAVEN_VERSION=3.8.4
# Tue, 23 Nov 2021 01:04:30 GMT
ARG USER_HOME_DIR=/root
# Tue, 23 Nov 2021 01:04:30 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Tue, 23 Nov 2021 01:04:30 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Tue, 23 Nov 2021 01:05:11 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 23 Nov 2021 01:05:11 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 23 Nov 2021 01:05:12 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 23 Nov 2021 01:05:12 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 23 Nov 2021 01:05:12 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 23 Nov 2021 01:05:13 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 23 Nov 2021 01:05:13 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7ef5b4a4700901695d7489ffa25c9a36a0c54f7003664412a2a582dd362fa`  
		Last Modified: Fri, 01 Oct 2021 02:59:16 GMT  
		Size: 3.0 MB (2959872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d70a5bfa8e87d64a9f2b2f6fdedbe49d6f21667069866e8ba624a15c35ef98b`  
		Last Modified: Fri, 01 Oct 2021 03:00:12 GMT  
		Size: 165.5 MB (165531206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41735f21ab7abde0ccdaaa21e7ef1e4be9ca505d74acf544051edc9412672347`  
		Last Modified: Tue, 23 Nov 2021 01:12:26 GMT  
		Size: 39.8 MB (39799490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1399f1e199a3bcb85247d146d7420b304d156d40876cff3b7ae60083da8db64`  
		Last Modified: Tue, 23 Nov 2021 01:12:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74957b9b0ce2a015ac77ba6da5b65f96312226473b8ea9f1dd66bc8875fbb4f5`  
		Last Modified: Tue, 23 Nov 2021 01:12:22 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibmjava` - linux; 386

```console
$ docker pull maven@sha256:db71879f7b8c2d2cf8e4350941de6e3757a08ef2d8f54ad4fbe4ee2794465ef2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.6 MB (220645525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d802ce4dc0fb1e16e3734aa1735ee415860d9332b8cf8f2715cb357e1c10c60`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 01 Oct 2021 03:46:35 GMT
ADD file:6718b956b86d332e4a53184568ac5205e92f9edeba804c64254e3b2da6e66c72 in / 
# Fri, 01 Oct 2021 03:46:36 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:22:39 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 04:22:46 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:22:46 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 04:24:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='953586dcb1870406d51fc0f346e2be062471d7dc67dce21ba2009cff0a46724f';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='09705ba9b6c53105062fd7764f9a066bfe5e2f58a64662d29c1eb030d51252e1';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e233b23f00ecda6a8e8fffe4b7c0675c3574754d300b680e70f423a60d047874';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e81cde52da8dd39160a70c98453e379f1286bb39e58f01ba94a63e45e31e2d34';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='dfc67c2861e00265140287091a713496840f5793946e087825f96c7afd4a8a50';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 04:25:00 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Oct 2021 19:20:36 GMT
ARG MAVEN_VERSION=3.8.3
# Wed, 06 Oct 2021 19:20:36 GMT
ARG USER_HOME_DIR=/root
# Wed, 06 Oct 2021 19:20:36 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Wed, 06 Oct 2021 19:20:36 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Wed, 06 Oct 2021 19:21:13 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 06 Oct 2021 19:21:13 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 06 Oct 2021 19:21:14 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 06 Oct 2021 19:21:14 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 06 Oct 2021 19:21:14 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 06 Oct 2021 19:21:14 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 06 Oct 2021 19:21:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:96391085795d2daa9755c58002e78a76eecf7fd57a1d8a3778e87b0079ed47e9`  
		Last Modified: Fri, 01 Oct 2021 03:47:35 GMT  
		Size: 27.2 MB (27158466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfd8a2f00fd7231d93b6eab959a6ea65acafe045c09e9e0602b1ea4293dd6c2`  
		Last Modified: Fri, 01 Oct 2021 04:25:31 GMT  
		Size: 3.0 MB (2988884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b25b2d568fc535899c14f210de6b8b399d2cc3d41fca90feab7f10fc3ae4b9`  
		Last Modified: Fri, 01 Oct 2021 04:26:36 GMT  
		Size: 153.7 MB (153740763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80913a5df4eb7834b0ded50205327f46ed006380f3d3a7f7adf9fec25e2f7fef`  
		Last Modified: Wed, 06 Oct 2021 19:21:47 GMT  
		Size: 36.8 MB (36756201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a0bddef5c80ad6478cf96f7942cfe1567e2611f833ba2845dc0eccddc9968c`  
		Last Modified: Wed, 06 Oct 2021 19:21:42 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891aac79667fc657d0e7a089ee6b72434d51df8f798de63eba14880f1682838e`  
		Last Modified: Wed, 06 Oct 2021 19:21:42 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibmjava` - linux; ppc64le

```console
$ docker pull maven@sha256:42b288d015144504763fbab6cff5f55f175d613ee8584d5c2d0718508318a333
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232853563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1030bfa7def99f631a5d411c9384f5893764c956e3bcec0e58b38ff5b97ab60c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:55:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Oct 2021 17:56:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:56:16 GMT
ENV JAVA_VERSION=8.0.6.36
# Wed, 06 Oct 2021 18:00:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='953586dcb1870406d51fc0f346e2be062471d7dc67dce21ba2009cff0a46724f';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='09705ba9b6c53105062fd7764f9a066bfe5e2f58a64662d29c1eb030d51252e1';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e233b23f00ecda6a8e8fffe4b7c0675c3574754d300b680e70f423a60d047874';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e81cde52da8dd39160a70c98453e379f1286bb39e58f01ba94a63e45e31e2d34';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='dfc67c2861e00265140287091a713496840f5793946e087825f96c7afd4a8a50';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Oct 2021 18:00:51 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Tue, 23 Nov 2021 00:45:47 GMT
ARG MAVEN_VERSION=3.8.4
# Tue, 23 Nov 2021 00:45:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 23 Nov 2021 00:45:50 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Tue, 23 Nov 2021 00:45:51 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Tue, 23 Nov 2021 00:46:24 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 23 Nov 2021 00:46:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 23 Nov 2021 00:46:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 23 Nov 2021 00:46:28 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 23 Nov 2021 00:46:29 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 23 Nov 2021 00:46:30 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 23 Nov 2021 00:46:32 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6e130fd3d09fd3fe6d741e0fa3f77120aa82717cf6d0a1cb49439939243a6`  
		Last Modified: Wed, 06 Oct 2021 18:04:08 GMT  
		Size: 3.1 MB (3081580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f598ff8622114dbbf1ac9528351f03df5c8f0844a529449c45dffea020111a62`  
		Last Modified: Wed, 06 Oct 2021 18:05:16 GMT  
		Size: 165.2 MB (165170269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4426392e0d5f67f84e996fb5fe36f9a4793c44f880769238652025d3b7b2ab`  
		Last Modified: Tue, 23 Nov 2021 00:49:20 GMT  
		Size: 34.2 MB (34167579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db9112d46024bd7ccc54535fe005639df43c6ae677457a68270f30449c9635a`  
		Last Modified: Tue, 23 Nov 2021 00:49:15 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bd89b5cc8d492e5006d38755a611c5d7946ea817001a589fcaa3006230530c`  
		Last Modified: Tue, 23 Nov 2021 00:49:15 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibmjava` - linux; s390x

```console
$ docker pull maven@sha256:09ec2f837fc59513350c072778d0518ab0d63ab81cd33a976bc89d02ab2cfc37
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.9 MB (215894179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b315c9fd8025ea8c2bc58ee11a668e969b153a8312f786ac20e5ae569d2811f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:23:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:23:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:37 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:25:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='953586dcb1870406d51fc0f346e2be062471d7dc67dce21ba2009cff0a46724f';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='09705ba9b6c53105062fd7764f9a066bfe5e2f58a64662d29c1eb030d51252e1';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e233b23f00ecda6a8e8fffe4b7c0675c3574754d300b680e70f423a60d047874';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e81cde52da8dd39160a70c98453e379f1286bb39e58f01ba94a63e45e31e2d34';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='dfc67c2861e00265140287091a713496840f5793946e087825f96c7afd4a8a50';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:25:51 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Tue, 23 Nov 2021 01:04:05 GMT
ARG MAVEN_VERSION=3.8.4
# Tue, 23 Nov 2021 01:04:05 GMT
ARG USER_HOME_DIR=/root
# Tue, 23 Nov 2021 01:04:05 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Tue, 23 Nov 2021 01:04:05 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Tue, 23 Nov 2021 01:04:24 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 23 Nov 2021 01:04:25 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 23 Nov 2021 01:04:25 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 23 Nov 2021 01:04:25 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 23 Nov 2021 01:04:26 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 23 Nov 2021 01:04:26 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 23 Nov 2021 01:04:26 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf425722012c2264c66ba97a53ff25a2f196330fbcc0872474e5e4562fa95f0`  
		Last Modified: Fri, 01 Oct 2021 02:27:43 GMT  
		Size: 2.7 MB (2676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3d9e09f0d1a147988e4b3a76835bc5965456062e5ded148222a25944881787`  
		Last Modified: Fri, 01 Oct 2021 02:28:26 GMT  
		Size: 155.7 MB (155677712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9b9b51c2d9119c80b6dff495ea9c6b15e6db19e8b6e5156027b1aff9d80a1b`  
		Last Modified: Tue, 23 Nov 2021 01:06:08 GMT  
		Size: 32.2 MB (32175968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23eae2d379e8fcc9fb5e9f6fc2b22377484058dff7cfc19e8be0e5d7e4ab7cb8`  
		Last Modified: Tue, 23 Nov 2021 01:06:05 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ec2327d03dfe2343ddb2f86df059ae46e43c4ceeb5e6934a65523895b0444`  
		Last Modified: Tue, 23 Nov 2021 01:06:05 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
