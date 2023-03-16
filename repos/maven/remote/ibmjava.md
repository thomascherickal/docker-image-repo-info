## `maven:ibmjava`

```console
$ docker pull maven@sha256:6d64efd9b922e9b8ce96eae4d398c13ee2ed73e4813cfa5933521f94148377a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `maven:ibmjava` - linux; amd64

```console
$ docker pull maven@sha256:20e66f71336c2fc8d63b2b15c7d403011bc0410347eb974e187cfbd3ef9d28c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.6 MB (208579036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e13394c3e1bdc6167a70d2ce77900299d0ea2d300d9e7adcb3f3b9b7d662f4`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:36:37 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Mar 2023 03:36:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:36:47 GMT
ENV JAVA_VERSION=8.0.7.20
# Thu, 16 Mar 2023 03:39:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='0f6aef4c3550a8f85288da8bc6fada405b0ce2226d6b1b57d0aae98cd5eef5e4';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='fa7661c2eb2982c4fb85c6894e7a975970b27b6ee82d5facb352f075cc1dfca3';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a56803671fe7d1c85f18d566dbcb7fbaf1d60c6f1d6de34e35a257e0c8095f9b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='71c913a1eed7daae952657e18eb9a2e71723106b6e7b56373f18564db77f551e';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='c8641bc22443ebccaedf1822a12ec1303d89577d45c875702e1f628066c7f383';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Mar 2023 03:39:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 16 Mar 2023 19:22:55 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 16 Mar 2023 19:22:55 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 16 Mar 2023 19:22:55 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 16 Mar 2023 19:22:55 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 16 Mar 2023 19:22:55 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 16 Mar 2023 19:22:55 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 16 Mar 2023 19:22:55 GMT
ARG MAVEN_VERSION=3.9.0
# Thu, 16 Mar 2023 19:22:55 GMT
ARG USER_HOME_DIR=/root
# Thu, 16 Mar 2023 19:22:55 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 16 Mar 2023 19:22:55 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 16 Mar 2023 19:22:55 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe43ddc3a069d2f66d64b9128ad2efde0e85efb6f720a7c7be3af6c784fe4211`  
		Last Modified: Thu, 16 Mar 2023 03:40:10 GMT  
		Size: 3.0 MB (2952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754e7019336ab7b425ccedb413d2212e49ac0b5c3e991b6d0215379733f80ab4`  
		Last Modified: Thu, 16 Mar 2023 03:40:56 GMT  
		Size: 166.5 MB (166474225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb7126bdbfbd051e98f18123be39a2373c11ef9f8f94c583941468338302451`  
		Last Modified: Thu, 16 Mar 2023 19:29:33 GMT  
		Size: 3.3 MB (3349594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b00ed18abf21f3a09b4eb4182a175bd325be808ce4e2afe6537ee5a17f9f08`  
		Last Modified: Thu, 16 Mar 2023 19:29:34 GMT  
		Size: 9.1 MB (9090722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51694cc2788cef69199cfc2e8a9817c755985666c4e3e781b7d27b78e1fe459e`  
		Last Modified: Thu, 16 Mar 2023 19:29:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e573b34e20fa8588832c1aacd4a0b5a08a9773e7eaa0bd78ea4ee637336250`  
		Last Modified: Thu, 16 Mar 2023 19:29:32 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acadd447b4b48af436804ec8604720b836722e1f81e06319d6118bdfdadf8af8`  
		Last Modified: Thu, 16 Mar 2023 19:29:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; ppc64le

```console
$ docker pull maven@sha256:4fdb072490c3365d5a4fa78995389baf8dbd9fa4f6855ab062a82c0e9873188d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.5 MB (212523157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cfd4eb408b8f56b1dfe6d32a5ba18af16ddfbb1b1a5c3e0fa5b5653487f549e`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:34:29 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Mar 2023 01:34:56 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:34:57 GMT
ENV JAVA_VERSION=8.0.7.20
# Thu, 16 Mar 2023 01:42:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='0f6aef4c3550a8f85288da8bc6fada405b0ce2226d6b1b57d0aae98cd5eef5e4';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='fa7661c2eb2982c4fb85c6894e7a975970b27b6ee82d5facb352f075cc1dfca3';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a56803671fe7d1c85f18d566dbcb7fbaf1d60c6f1d6de34e35a257e0c8095f9b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='71c913a1eed7daae952657e18eb9a2e71723106b6e7b56373f18564db77f551e';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='c8641bc22443ebccaedf1822a12ec1303d89577d45c875702e1f628066c7f383';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Mar 2023 01:42:17 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 16 Mar 2023 19:22:02 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 16 Mar 2023 19:22:02 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 16 Mar 2023 19:22:02 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 16 Mar 2023 19:22:03 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 16 Mar 2023 19:22:03 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 16 Mar 2023 19:22:04 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 16 Mar 2023 19:22:04 GMT
ARG MAVEN_VERSION=3.9.0
# Thu, 16 Mar 2023 19:22:04 GMT
ARG USER_HOME_DIR=/root
# Thu, 16 Mar 2023 19:22:04 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 16 Mar 2023 19:22:04 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 16 Mar 2023 19:22:04 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a045bec75deb795fa894947efc21348c99f3e44cd0e657cf75429ed5eede9b51`  
		Last Modified: Thu, 16 Mar 2023 01:42:54 GMT  
		Size: 3.1 MB (3077290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f476f9d91d88f829ec3c8873c16fa520b0e8f8e3a872fa50b226af07912dac92`  
		Last Modified: Thu, 16 Mar 2023 01:44:06 GMT  
		Size: 166.3 MB (166271826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c256984388b34934c87ea1070312eef3176a6e4f614059576f6b4523568db56`  
		Last Modified: Thu, 16 Mar 2023 19:30:01 GMT  
		Size: 3.6 MB (3640003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8308a8e94399f86b49cda0dc1c8b67bef1a59b91156b6c623e6c6e127da9db`  
		Last Modified: Thu, 16 Mar 2023 19:30:00 GMT  
		Size: 9.1 MB (9090726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf66e3aff13522e4672fc8d687d428c3c8cc37dd182e850be812848a1560319`  
		Last Modified: Thu, 16 Mar 2023 19:29:59 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03dacb16b828c0f78202d15fe94c2654601a9064267a9d44ca31eac0ca47ed12`  
		Last Modified: Thu, 16 Mar 2023 19:29:59 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc214f98e1259018b2f7c25fdb89a779681b1e9c277c085d2b8523e2e8dd2d3`  
		Last Modified: Thu, 16 Mar 2023 19:29:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; s390x

```console
$ docker pull maven@sha256:299f20272c1a0e026d19c27c08faf4ba044250bbf1af93a7afa2afa37e27dca7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197219219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddaf41336cc630f2daec01377df06c9f68af5f4f25fd4a94366dc7277defc75c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 08 Mar 2023 03:23:29 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:23:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:23:31 GMT
ADD file:a6309e462d28398152cb726a11615118d79858da963b8c614772b87d87465967 in / 
# Wed, 08 Mar 2023 03:23:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:38:18 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Mar 2023 02:38:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:38:24 GMT
ENV JAVA_VERSION=8.0.7.20
# Thu, 16 Mar 2023 02:43:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='0f6aef4c3550a8f85288da8bc6fada405b0ce2226d6b1b57d0aae98cd5eef5e4';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='fa7661c2eb2982c4fb85c6894e7a975970b27b6ee82d5facb352f075cc1dfca3';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a56803671fe7d1c85f18d566dbcb7fbaf1d60c6f1d6de34e35a257e0c8095f9b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='71c913a1eed7daae952657e18eb9a2e71723106b6e7b56373f18564db77f551e';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='c8641bc22443ebccaedf1822a12ec1303d89577d45c875702e1f628066c7f383';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Mar 2023 02:43:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 16 Mar 2023 21:27:46 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 16 Mar 2023 21:27:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 16 Mar 2023 21:27:46 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 16 Mar 2023 21:27:46 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 16 Mar 2023 21:27:46 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 16 Mar 2023 21:27:47 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 16 Mar 2023 21:27:47 GMT
ARG MAVEN_VERSION=3.9.0
# Thu, 16 Mar 2023 21:27:47 GMT
ARG USER_HOME_DIR=/root
# Thu, 16 Mar 2023 21:27:47 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 16 Mar 2023 21:27:47 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 16 Mar 2023 21:27:47 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3a2279f06ab19f0d57823e69b999f54a344e28bd9f955b4db9a5875c0caa543a`  
		Last Modified: Thu, 16 Mar 2023 02:01:03 GMT  
		Size: 25.4 MB (25370993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c6fa88382e166a9b693d8b861f913ff7b356af9dff894ad987e650a41f3335`  
		Last Modified: Thu, 16 Mar 2023 02:44:12 GMT  
		Size: 2.7 MB (2668974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395f1e8a910b3d6d2bc060348c48a8dccc7e4e86819d1685d9ac354bc1c41dbb`  
		Last Modified: Thu, 16 Mar 2023 02:44:52 GMT  
		Size: 156.8 MB (156764109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc51125cd7f858667a14a119ce514a6e79b738cbe20362fab591ee5d818c0a8`  
		Last Modified: Thu, 16 Mar 2023 21:31:10 GMT  
		Size: 3.3 MB (3323075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5805646aa113cc5519951d61042111f9682ada3ece8e545e9928fea8050b0ab5`  
		Last Modified: Thu, 16 Mar 2023 21:31:10 GMT  
		Size: 9.1 MB (9090703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71cf4dd24ff43860732187f42851a0baf41833fe0fda424cb9e24decf1e631c`  
		Last Modified: Thu, 16 Mar 2023 21:31:09 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6194acbb8e48c7019fa0b360944783d2addda37d1d7de03d9c8b0fef259d7303`  
		Last Modified: Thu, 16 Mar 2023 21:31:09 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0911f6ec1044e9af62450dc46699cf12b53788618c282d11bef1d13b499d2d37`  
		Last Modified: Thu, 16 Mar 2023 21:31:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
