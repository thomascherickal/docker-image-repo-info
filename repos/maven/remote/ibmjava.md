## `maven:ibmjava`

```console
$ docker pull maven@sha256:9dec2ac6e6fec0f7e5da327ef58c4eea2d1bcee4fa45799ef3e1ddd628730421
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `maven:ibmjava` - linux; amd64

```console
$ docker pull maven@sha256:c1956dbd1f4e0217a7bf8bf6a71237f465250be5cc9fb6e03b2e92cc18bf77fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.1 MB (214134140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:975b93c08fdad67c98e4b524d0539d6c5b46306083268d02b95730968550dcff`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:57:15 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 16 Jun 2023 02:57:21 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:57:21 GMT
ENV JAVA_VERSION=8.0.8.5
# Fri, 16 Jun 2023 03:00:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='a1b462fd16ae935c34523b761a08010120c074d10cd7ac339af213a9bed59f05';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='eac7923675423ef01db312a59ee68c96eb8ec474560630bda4d24807d4980dcf';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='9e14a91a5cd4aaafe5553b06364249cd7819d31edf187e1160ca6bec5ce3a82b';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='995373f2d4395484e8c784fe39062e98b5f6f6cb1a90ae6dd8931b7bfdc6cb14';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 16 Jun 2023 03:00:49 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Mon, 26 Jun 2023 13:48:06 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ARG MAVEN_VERSION=3.9.3
# Mon, 26 Jun 2023 13:48:06 GMT
ARG USER_HOME_DIR=/root
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 26 Jun 2023 13:48:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 26 Jun 2023 13:48:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1aab967c9f4d601afc5e8b2023fa6a57cdb9f402102cbf9e941ffab60ec77b`  
		Last Modified: Fri, 16 Jun 2023 03:01:13 GMT  
		Size: 1.5 MB (1469042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e999be3e47e84f8318ec04aa00141d2d30eb83aa56907132259042e6bb23864c`  
		Last Modified: Fri, 16 Jun 2023 03:01:58 GMT  
		Size: 171.2 MB (171210150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9fad6cf4c0e45e4f0facd198e9f94d289b7afda8cd8bcb5a82cace4c8aee35`  
		Last Modified: Fri, 16 Jun 2023 07:29:40 GMT  
		Size: 1.7 MB (1694984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54cf36d80880c3e9479c5bc27424f86e5bd9d64d2a53a63e8e9091b6446c902e`  
		Last Modified: Tue, 27 Jun 2023 01:16:50 GMT  
		Size: 9.3 MB (9327559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dcdef1269e79ca9c9c86e16f8df0f827dbcdaa89aacdd3462aff14d070ffed`  
		Last Modified: Tue, 27 Jun 2023 01:16:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c7abe32abb7d51db3c09af027eb93b1ab8c067654a54c153cf2ba890274d7`  
		Last Modified: Tue, 27 Jun 2023 01:16:49 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1901ebf466397d185ccf909dd54b9345302995ecd7914a010c82cded22de834`  
		Last Modified: Tue, 27 Jun 2023 01:16:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; ppc64le

```console
$ docker pull maven@sha256:48d49440f7f5efedcd5daeb0abcf06d23ae9ec3e4ac0dd5980e1cc6bd39f0b8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219703617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c8f08f995cce5ecb3ad81c86bfcc2d38128e2506a30db2ee93f8a8a36b2a5f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:00 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:03 GMT
ADD file:00c4f44b35b683caef54d5b8b0e0b1e68872f45eae17dd7543adaf6c54512447 in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:32:04 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 16 Jun 2023 01:32:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:32:19 GMT
ENV JAVA_VERSION=8.0.8.5
# Fri, 16 Jun 2023 01:40:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='a1b462fd16ae935c34523b761a08010120c074d10cd7ac339af213a9bed59f05';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='eac7923675423ef01db312a59ee68c96eb8ec474560630bda4d24807d4980dcf';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='9e14a91a5cd4aaafe5553b06364249cd7819d31edf187e1160ca6bec5ce3a82b';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='995373f2d4395484e8c784fe39062e98b5f6f6cb1a90ae6dd8931b7bfdc6cb14';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 16 Jun 2023 01:40:20 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Mon, 26 Jun 2023 13:48:06 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ARG MAVEN_VERSION=3.9.3
# Mon, 26 Jun 2023 13:48:06 GMT
ARG USER_HOME_DIR=/root
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 26 Jun 2023 13:48:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 26 Jun 2023 13:48:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a02dd69d9a8a1e6f4fc2ccb509fb8efd6014b00ff932a757d23b4b012a2bec49`  
		Last Modified: Fri, 16 Jun 2023 00:44:52 GMT  
		Size: 35.7 MB (35711397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3831c1123275dd4d9043ad21bf2c9fb47b24b3ab61e99547e14106df60427380`  
		Last Modified: Fri, 16 Jun 2023 01:40:42 GMT  
		Size: 1.6 MB (1576481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260406cb1e7fd613b7e09eeaa2a51135d336a5e8cbec3975859139fa201c68a1`  
		Last Modified: Fri, 16 Jun 2023 01:41:49 GMT  
		Size: 171.0 MB (171028804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653cf3ca760adb678e7b0f64828675adc4fa8a8a732ac8e50d22619ad1d88958`  
		Last Modified: Fri, 16 Jun 2023 02:55:31 GMT  
		Size: 2.1 MB (2057993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e1b42143156d435263c40e3ae485151fc96b8e00a8fab92f12a6d1284adcb8`  
		Last Modified: Tue, 27 Jun 2023 02:17:20 GMT  
		Size: 9.3 MB (9327571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94af14a2176464a6f1868ee75122f268f1c0bc4e3219dc9c2af3045e338cb4b`  
		Last Modified: Tue, 27 Jun 2023 02:17:19 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35eeb9d1dd9bb73c8a53f228d5bfadc7bc910f08d0f15e8d7f50f54482e91fce`  
		Last Modified: Tue, 27 Jun 2023 02:17:19 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82462307a7e7e83690be032f45a59c6ac024a267358c65305d9b4f4351815c87`  
		Last Modified: Tue, 27 Jun 2023 02:17:19 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; s390x

```console
$ docker pull maven@sha256:687ebd6300a342ee1e8ab88d7b1c54657f0c551a9ff13d72527cb4edd309eaab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202065841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d7ab5d488ffe2d20f12ffa7d3546c92d8652bf1fae4be4ebc5bfcdec3316e7`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:02 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:02 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:04 GMT
ADD file:2d2f31ec110b9e7ec21a9d4824a430acdaabf0b4e9c1cdd337438992859b57ae in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 18:25:52 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 16 Jun 2023 18:25:56 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 30 Jun 2023 22:42:14 GMT
ENV JAVA_VERSION=8.0.8.6
# Fri, 30 Jun 2023 22:45:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bd95ba315fa0752be3a18fd67c0dbda568313484f21420999766bc46c9af9191';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e159747a1fe64a03a24994887c8e4ab3aea06072f3a2ed99c3db31cec0c224de';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='7385da0c5ffde5b81f4830b95aa352db2a89b8380ccef25dcd77fdf5b0af3488';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='096edb7671f217d64ec9a6cf44b4d0e7f56184da1aa32e8d84eebe36c02c80d9';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 30 Jun 2023 22:45:05 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Mon, 26 Jun 2023 13:48:06 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ARG MAVEN_VERSION=3.9.3
# Mon, 26 Jun 2023 13:48:06 GMT
ARG USER_HOME_DIR=/root
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 26 Jun 2023 13:48:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 26 Jun 2023 13:48:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:fab1a8aa44b00432834b7776a76fd4149ec2fee2336a3521bd5435428df7edc9`  
		Last Modified: Fri, 16 Jun 2023 18:23:35 GMT  
		Size: 28.6 MB (28644581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1521659225e331fd6923943db586c259687a2b65eab1dbc35fce49da80029f3`  
		Last Modified: Fri, 16 Jun 2023 18:37:39 GMT  
		Size: 1.5 MB (1477026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d8e951ec17c9a3c7a70b7e137b59cb0af83aaba951a0c9ab3aa7b960887c9d`  
		Last Modified: Fri, 30 Jun 2023 22:46:04 GMT  
		Size: 160.9 MB (160926181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96334a10f69ae442c1fa1fa1a33f78eaf6399e5cc5817aef6054bd2c34266d7f`  
		Last Modified: Fri, 30 Jun 2023 23:02:40 GMT  
		Size: 1.7 MB (1689117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de29434e8232831a8e5ba41eeaf87c5c5ce360b8cddd82cd78c6bcd997f1be0c`  
		Last Modified: Fri, 30 Jun 2023 23:02:40 GMT  
		Size: 9.3 MB (9327563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fcdd404222f0827e76ee9138f41c575d02f61f9f4a2166931c08e1eeeb4db6c`  
		Last Modified: Fri, 30 Jun 2023 23:02:40 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dc4a195cb9be88aec9ec30df500993a7e779db70f04119fa6b9223fa09ffc9`  
		Last Modified: Fri, 30 Jun 2023 23:02:40 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d18a834b545d27b327fe21ca73c76f7facff5fc8c94c41360cf5ad7da0c2c9`  
		Last Modified: Fri, 30 Jun 2023 23:02:40 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
