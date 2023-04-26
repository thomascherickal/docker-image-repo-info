## `maven:ibmjava`

```console
$ docker pull maven@sha256:df66dd15f5fbe4b9e0c0ef0bceb8ae85b0a844543bf067fcbd364560fd54d103
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `maven:ibmjava` - linux; amd64

```console
$ docker pull maven@sha256:4e98b651e853b5cb56ae9cc585d80ec8d6af98c2b4114a7aa7e2196b04be1f26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.7 MB (213681353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc1059b94df88fc519119c9625319e418ac5bc036250cbfe3b0704644699a453`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 22:19:33 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 31 Mar 2023 22:19:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 31 Mar 2023 22:19:41 GMT
ENV JAVA_VERSION=8.0.8.0
# Fri, 31 Mar 2023 22:22:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='8a1dfef941fc2e43fcd8143960d2c3a82e283695eff893923cb05c226bcdd0a0';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5a3d2ef0ad3687b34e1df3854b45d2e00a034724fe70a0e5bf14b2eebca1fe9b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f361174227db6e6e1b067b8085549fd2f7ba63a73752a2db7be260e438ef39eb';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='974c339555e219ea93198316f6a33ee8243481e568a730d68b467c79f7caa5bc';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 31 Mar 2023 22:22:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 26 Apr 2023 19:21:32 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 26 Apr 2023 19:21:32 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 26 Apr 2023 19:21:32 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Wed, 26 Apr 2023 19:21:32 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Wed, 26 Apr 2023 19:21:32 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Wed, 26 Apr 2023 19:21:32 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Wed, 26 Apr 2023 19:21:32 GMT
ARG MAVEN_VERSION=3.9.1
# Wed, 26 Apr 2023 19:21:32 GMT
ARG USER_HOME_DIR=/root
# Wed, 26 Apr 2023 19:21:32 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 26 Apr 2023 19:21:32 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 26 Apr 2023 19:21:32 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76592b838d832d2f6a0e0691d8d3efa85fffa35e81c119bed83fd87227183a5f`  
		Last Modified: Fri, 31 Mar 2023 22:23:03 GMT  
		Size: 1.4 MB (1446443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c52385b7867beb91dd8bbd0701460150377d314e0a1826704a63951c53785f8`  
		Last Modified: Fri, 31 Mar 2023 22:23:47 GMT  
		Size: 171.0 MB (171003209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a974008e3974ea2b1fed2cfb8be8ed782985916dafa8e828335ce5a119fa5b5d`  
		Last Modified: Fri, 31 Mar 2023 22:40:41 GMT  
		Size: 1.7 MB (1694210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6baefda3ff5eeb9ea237aa02f955ee913f61ff38b2edadbbdb0ff5306a25133`  
		Last Modified: Wed, 05 Apr 2023 17:31:40 GMT  
		Size: 9.1 MB (9106159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e23fbffcba17464747f9ee7145050b5d8bf21c3e20ae2ccfaa86a8478ce39a3`  
		Last Modified: Wed, 05 Apr 2023 17:31:39 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de4e2b0080be1600a3e59471e4bd0e4bae2962a242166ef4573e28c7a1ac0f`  
		Last Modified: Wed, 05 Apr 2023 17:31:39 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a70c190f482f8b4f7a14b0cd619f2b2540d1fd350ac10eed5398cd8891345b5`  
		Last Modified: Wed, 05 Apr 2023 17:31:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; ppc64le

```console
$ docker pull maven@sha256:1fb3c6aedcdffe5b2d2359c343f4d5933f21a1b77a0e6585c38fcfce532c56ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.3 MB (219266385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df18874b4f24c7b35d8f2b8d8e39ab6a59bbe28912d49f75dd798cf57657bc0`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 22:21:07 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 31 Mar 2023 22:21:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 31 Mar 2023 22:21:31 GMT
ENV JAVA_VERSION=8.0.8.0
# Fri, 31 Mar 2023 22:29:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='8a1dfef941fc2e43fcd8143960d2c3a82e283695eff893923cb05c226bcdd0a0';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5a3d2ef0ad3687b34e1df3854b45d2e00a034724fe70a0e5bf14b2eebca1fe9b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f361174227db6e6e1b067b8085549fd2f7ba63a73752a2db7be260e438ef39eb';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='974c339555e219ea93198316f6a33ee8243481e568a730d68b467c79f7caa5bc';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 31 Mar 2023 22:29:29 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 26 Apr 2023 19:20:17 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 26 Apr 2023 19:20:17 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 26 Apr 2023 19:20:17 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Wed, 26 Apr 2023 19:20:17 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Wed, 26 Apr 2023 19:20:17 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Wed, 26 Apr 2023 19:20:17 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Wed, 26 Apr 2023 19:20:17 GMT
ARG MAVEN_VERSION=3.9.1
# Wed, 26 Apr 2023 19:20:17 GMT
ARG USER_HOME_DIR=/root
# Wed, 26 Apr 2023 19:20:17 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 26 Apr 2023 19:20:17 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 26 Apr 2023 19:20:17 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:deffc758660db3b0ee7a1f211d720633f06f27ab1e4c31db4caf8c27f4a80eeb`  
		Last Modified: Thu, 16 Mar 2023 02:22:27 GMT  
		Size: 35.7 MB (35711728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edde4d0991b2fc61228d445220b004d843c08e4eb5f5dba26f3e2f7edaf14848`  
		Last Modified: Fri, 31 Mar 2023 22:29:44 GMT  
		Size: 1.6 MB (1552384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da20ab43d4a941d94eb56f0fedec6009864287a98dea398ea6b7a838e25d8a34`  
		Last Modified: Fri, 31 Mar 2023 22:30:53 GMT  
		Size: 170.8 MB (170838489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6168baecc731bd042bc37bdb0ba2d7cf2271f51c9c41cf1b1d5dbdc646eaf64`  
		Last Modified: Fri, 31 Mar 2023 22:47:48 GMT  
		Size: 2.1 MB (2056276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e65049f9202b3d41ece2da1c8066b1ea91ece42addfea6fe83061eb46f2dcda`  
		Last Modified: Wed, 05 Apr 2023 17:28:04 GMT  
		Size: 9.1 MB (9106140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b50400c4128f2ff7300a94f464f040ca652adbca9d317cd9e087cf1dc50a658`  
		Last Modified: Wed, 05 Apr 2023 17:28:03 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b037f04b4256b3e90d968bc781a1779a2f70f1ff3f6c465d5a545cf5e02b66`  
		Last Modified: Wed, 05 Apr 2023 17:28:03 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546ddc1785c85483f4a682ff585be4b247016ecfb4a91c734aeb83b9e7e32ca6`  
		Last Modified: Wed, 05 Apr 2023 17:28:02 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; s390x

```console
$ docker pull maven@sha256:62d4f9a8f9670e9b77b3ec0b17d65848ab209676874b2a760fb10782c00af0a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.9 MB (201850271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a2701bd56d5aa215d68182b0ba8627a4882b791804ebe79f9e7206b37b34eb4`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 21:42:09 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 31 Mar 2023 21:42:22 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 31 Mar 2023 21:42:22 GMT
ENV JAVA_VERSION=8.0.8.0
# Fri, 31 Mar 2023 21:45:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='8a1dfef941fc2e43fcd8143960d2c3a82e283695eff893923cb05c226bcdd0a0';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5a3d2ef0ad3687b34e1df3854b45d2e00a034724fe70a0e5bf14b2eebca1fe9b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f361174227db6e6e1b067b8085549fd2f7ba63a73752a2db7be260e438ef39eb';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='974c339555e219ea93198316f6a33ee8243481e568a730d68b467c79f7caa5bc';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 31 Mar 2023 21:45:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 26 Apr 2023 19:42:27 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 26 Apr 2023 19:42:27 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 26 Apr 2023 19:42:27 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Wed, 26 Apr 2023 19:42:27 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Wed, 26 Apr 2023 19:42:27 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Wed, 26 Apr 2023 19:42:27 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Wed, 26 Apr 2023 19:42:27 GMT
ARG MAVEN_VERSION=3.9.1
# Wed, 26 Apr 2023 19:42:27 GMT
ARG USER_HOME_DIR=/root
# Wed, 26 Apr 2023 19:42:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 26 Apr 2023 19:42:27 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 26 Apr 2023 19:42:27 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:2c7366af510b72cc0b3456fb93cfa0bfc76f7d383db5cb315967e7b1ce2e0c42`  
		Last Modified: Thu, 16 Mar 2023 02:02:40 GMT  
		Size: 28.6 MB (28647599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e458936873e72c656dd508c3163aeef4a5e866071e6fc64d093fee431ee1683`  
		Last Modified: Fri, 31 Mar 2023 21:45:26 GMT  
		Size: 1.5 MB (1452441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed239bc4c4e45ef570aabff4beac9769025a0c7402b6227bc9ed7a2886ac017`  
		Last Modified: Fri, 31 Mar 2023 21:46:02 GMT  
		Size: 161.0 MB (160954514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91451348c31722104d1f03e242ec4171a4dbadd8f93aef60e9eea78914accb4`  
		Last Modified: Fri, 31 Mar 2023 22:02:48 GMT  
		Size: 1.7 MB (1688193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b316db9be4aed5ffb5f6f55c6c6af3a23a333309fd7978ee920d87e5f10f10c5`  
		Last Modified: Wed, 05 Apr 2023 16:44:31 GMT  
		Size: 9.1 MB (9106160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9914640ddaeda5924adbd3710a1fc82dd711fc6c69230d5b8feb1f1bdcb8d8`  
		Last Modified: Wed, 05 Apr 2023 16:44:31 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9196d2c34fdb46725e9ae54344259833a3c9d28684bc3f5192e99bd9fcc29d9e`  
		Last Modified: Wed, 05 Apr 2023 16:44:31 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bca10bb633137a7610b985c03a2adc2dd96fedc97e266807d55583bd89d74e`  
		Last Modified: Wed, 05 Apr 2023 16:44:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
