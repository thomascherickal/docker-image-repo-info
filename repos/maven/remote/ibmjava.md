## `maven:ibmjava`

```console
$ docker pull maven@sha256:b38accd252f810a64cd659c7e95491f3f0943584cbbcd28a625f177b0f85bf11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `maven:ibmjava` - linux; amd64

```console
$ docker pull maven@sha256:7a39f92b93da5d16a506102c1affd7d01d1b102dc430cba8c2a5c3d626879690
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.4 MB (237373845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70c10c4f78e1e20997cea2151333972ad5eccafcf5741ed4e57cec60ea352dd7`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:09:52 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 20:10:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:10:01 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 20:12:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='8a5a580ae482fc1413feae44da07fe68acfbc9aafc911a781480e1752e3b4b94';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='565caead453b1b6ecec9a393cd298d407a2c07737e70db27b187cf4b4a7c1a62';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='d982a09d55481738f9e2fea9375ad55a72eb6a5069a5142cd2cb99b6db836ad3';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='0bab09c4fa8cafb2cb53444ab4c7649f2ba51691e76571de953235cbeaa45137';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='1795165f444421e63d8d6f6f4704c89368cf283c4984b00e29f152d823e2bf3c';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 20:12:58 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 07:37:12 GMT
RUN apt-get update && apt-get install -y curl
# Wed, 03 Aug 2022 07:37:12 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 03 Aug 2022 07:37:12 GMT
ARG USER_HOME_DIR=/root
# Wed, 03 Aug 2022 07:37:13 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 03 Aug 2022 07:37:13 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 03 Aug 2022 07:37:15 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 03 Aug 2022 07:37:15 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 03 Aug 2022 07:37:15 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 03 Aug 2022 07:37:15 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 03 Aug 2022 07:37:15 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 03 Aug 2022 07:37:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 03 Aug 2022 07:37:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6715a1bb89fcf5e91403be2bc6130f23e6b3cfd0da73e6b09e937d028409d3`  
		Last Modified: Tue, 02 Aug 2022 20:13:24 GMT  
		Size: 3.0 MB (2957815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e529d919225d24589455693c77fdf6d3f82e829482c096492f3f63f99a90fe57`  
		Last Modified: Tue, 02 Aug 2022 20:14:17 GMT  
		Size: 166.3 MB (166253742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defec794d735a424aac3b45b67c73ffd269894be9a5ba949a14dee4a6810b614`  
		Last Modified: Wed, 03 Aug 2022 07:44:55 GMT  
		Size: 32.7 MB (32711302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370bede70450c633a36eb3b31dbb63c882ae75c4d043201e262fa0a5993b8dff`  
		Last Modified: Wed, 03 Aug 2022 07:44:52 GMT  
		Size: 8.7 MB (8739504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995cac270acb3d872fd99b373732f48edd8cdc49fb2fb264e0993e2d5c3a670d`  
		Last Modified: Wed, 03 Aug 2022 07:44:52 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440e1953b2aee019361da92a3e9002eb1b10b8c020c570587b21d98edc0cf165`  
		Last Modified: Wed, 03 Aug 2022 07:44:52 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; 386

```console
$ docker pull maven@sha256:f2fc3292d7c61f705aa840858ca59bde56a0016fcfa9efe7bbaaf9a29d4ac16e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221319989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e09d44adaa0c06b9f02b73aeeacaa70bf6cb1b49be437e8cd6c89b31cd6b8439`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 02 Aug 2022 00:50:55 GMT
ADD file:6d22c6318075d01068d0a9213f33655abf6c251f8a71d98c17b857b9021b43bd in / 
# Tue, 02 Aug 2022 00:50:55 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:23:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 16:23:28 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:23:28 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 16:26:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='8a5a580ae482fc1413feae44da07fe68acfbc9aafc911a781480e1752e3b4b94';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='565caead453b1b6ecec9a393cd298d407a2c07737e70db27b187cf4b4a7c1a62';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='d982a09d55481738f9e2fea9375ad55a72eb6a5069a5142cd2cb99b6db836ad3';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='0bab09c4fa8cafb2cb53444ab4c7649f2ba51691e76571de953235cbeaa45137';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='1795165f444421e63d8d6f6f4704c89368cf283c4984b00e29f152d823e2bf3c';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 16:26:36 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Tue, 02 Aug 2022 22:43:05 GMT
RUN apt-get update && apt-get install -y curl
# Tue, 02 Aug 2022 22:43:05 GMT
ARG MAVEN_VERSION=3.8.6
# Tue, 02 Aug 2022 22:43:06 GMT
ARG USER_HOME_DIR=/root
# Tue, 02 Aug 2022 22:43:07 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Tue, 02 Aug 2022 22:43:08 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Tue, 02 Aug 2022 22:43:16 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 02 Aug 2022 22:43:17 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 02 Aug 2022 22:43:18 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 02 Aug 2022 22:43:20 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 02 Aug 2022 22:43:21 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 02 Aug 2022 22:43:21 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 02 Aug 2022 22:43:22 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5496b4c91dece81ce997c62cf2e1ef6f1764e612c6e8f0b385722c6645e4ad30`  
		Last Modified: Tue, 02 Aug 2022 00:51:39 GMT  
		Size: 27.2 MB (27164268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0dd584134d885dc07df56cb1531c30c56e50d96a7cc1cb92c61c41813d18e0`  
		Last Modified: Tue, 02 Aug 2022 16:27:10 GMT  
		Size: 3.0 MB (2983285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b94ea674a65dbc89f3785f80ee02e2df7da6d3bec5eb25f6a994ec9b0db5259`  
		Last Modified: Tue, 02 Aug 2022 16:28:16 GMT  
		Size: 154.4 MB (154359005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1668ca6caf761cfdbd0f312bbccbc9bf93f16b860633fe82778579f0571b28b`  
		Last Modified: Tue, 02 Aug 2022 22:43:51 GMT  
		Size: 28.1 MB (28072754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4396c08b57020c7901851af34111f7965715f7758d5b856210e2d0251e23ae87`  
		Last Modified: Tue, 02 Aug 2022 22:43:48 GMT  
		Size: 8.7 MB (8739464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4a9cda4b32b23d007c5f80a5a907b7502c0d6b3f87636df30be67edc943fed`  
		Last Modified: Tue, 02 Aug 2022 22:43:46 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84701d52ad9102c6ca654983e2fec12926da65270645b756bf45d4b69da8ac6`  
		Last Modified: Tue, 02 Aug 2022 22:43:46 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; ppc64le

```console
$ docker pull maven@sha256:e7399d506f936c18bca3d0b460e74ee6dee49fd893d43235b3b26ebaa2a63409
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.6 MB (233585555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d770a775bc9ca5ebdde70ba0f23d878b7d224e214bd18c5b85372e9792812e21`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:50 GMT
ADD file:32fc7b9b5853c93c45b1a96054c30104fd200ac7d40d0388aff736c478f917cb in / 
# Tue, 02 Aug 2022 01:30:52 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 03:44:16 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 03 Aug 2022 03:44:53 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 03:44:53 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 03 Aug 2022 03:52:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='8a5a580ae482fc1413feae44da07fe68acfbc9aafc911a781480e1752e3b4b94';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='565caead453b1b6ecec9a393cd298d407a2c07737e70db27b187cf4b4a7c1a62';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='d982a09d55481738f9e2fea9375ad55a72eb6a5069a5142cd2cb99b6db836ad3';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='0bab09c4fa8cafb2cb53444ab4c7649f2ba51691e76571de953235cbeaa45137';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='1795165f444421e63d8d6f6f4704c89368cf283c4984b00e29f152d823e2bf3c';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 03 Aug 2022 03:52:21 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 23:49:17 GMT
RUN apt-get update && apt-get install -y curl
# Wed, 03 Aug 2022 23:49:18 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 03 Aug 2022 23:49:18 GMT
ARG USER_HOME_DIR=/root
# Wed, 03 Aug 2022 23:49:18 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 03 Aug 2022 23:49:18 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 03 Aug 2022 23:49:21 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 03 Aug 2022 23:49:21 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 03 Aug 2022 23:49:21 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 03 Aug 2022 23:49:22 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 03 Aug 2022 23:49:22 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 03 Aug 2022 23:49:22 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 03 Aug 2022 23:49:23 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:1a9ff13e38cae7994b55e6db5c3d190d2b7a03043ae238a6f71a285376de46bb`  
		Last Modified: Tue, 02 Aug 2022 01:33:07 GMT  
		Size: 30.4 MB (30441470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99970d1735353adabddaef52faa1237908c9cdf39198088cf543cb21ecb3fa69`  
		Last Modified: Wed, 03 Aug 2022 03:52:54 GMT  
		Size: 3.1 MB (3075943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67704bb09f7471ac8c82135a0717b82e72dbe13a77b7046e405dd421b9c3609`  
		Last Modified: Wed, 03 Aug 2022 03:54:08 GMT  
		Size: 165.9 MB (165909904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad4aee9c999605990cf6497779fc00bb449ffbb6adbe5b462357e4a364729a1`  
		Last Modified: Wed, 03 Aug 2022 23:55:49 GMT  
		Size: 25.4 MB (25417543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba917c21e67bf9ae986b61c39f7cfb99e8892f232b9eb6ddefcda3a794af783`  
		Last Modified: Wed, 03 Aug 2022 23:55:46 GMT  
		Size: 8.7 MB (8739481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81342117a807dfb396c1640c293f39b60de974ab584e84adad2ab9fa0d75b8e1`  
		Last Modified: Wed, 03 Aug 2022 23:55:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faffd99f55030d9f91d5bf870c5b463a865e3064afbf45615498b183aa98794b`  
		Last Modified: Wed, 03 Aug 2022 23:55:45 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; s390x

```console
$ docker pull maven@sha256:0cb7cbab033ba4aa7622ebf67e375b605b0e4649570f592d4d678bf68daed9a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.6 MB (216613816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dac2ed8dea72f34ec653bf2a81577353a2192b892e0c5fc5c71b08847a11854`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 02 Aug 2022 01:01:57 GMT
ADD file:3d2e9b401524527b395347bc3847be7c9cb465b9a214a1a1d31e74330e293c45 in / 
# Tue, 02 Aug 2022 01:01:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:19:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 13:19:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:19:25 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 13:22:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='8a5a580ae482fc1413feae44da07fe68acfbc9aafc911a781480e1752e3b4b94';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='565caead453b1b6ecec9a393cd298d407a2c07737e70db27b187cf4b4a7c1a62';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='d982a09d55481738f9e2fea9375ad55a72eb6a5069a5142cd2cb99b6db836ad3';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='0bab09c4fa8cafb2cb53444ab4c7649f2ba51691e76571de953235cbeaa45137';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='1795165f444421e63d8d6f6f4704c89368cf283c4984b00e29f152d823e2bf3c';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 13:22:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:01:10 GMT
RUN apt-get update && apt-get install -y curl
# Wed, 03 Aug 2022 00:01:12 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 03 Aug 2022 00:01:13 GMT
ARG USER_HOME_DIR=/root
# Wed, 03 Aug 2022 00:01:14 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 03 Aug 2022 00:01:15 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 03 Aug 2022 00:01:29 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 03 Aug 2022 00:01:30 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 03 Aug 2022 00:01:31 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 03 Aug 2022 00:01:31 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 03 Aug 2022 00:01:32 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 03 Aug 2022 00:01:33 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 03 Aug 2022 00:01:33 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:be3ed498266c519f84268ff1f02085fa249c0e32fb60a59466e24c862b5f094b`  
		Last Modified: Tue, 02 Aug 2022 01:03:25 GMT  
		Size: 25.4 MB (25369584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2ed0adcefe11b30e3dff027bcb1cb9fe759f39f50b008bafb3644d3d2fcba8`  
		Last Modified: Tue, 02 Aug 2022 13:22:41 GMT  
		Size: 2.7 MB (2671706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfef873240c8f213f8f5a7c6d6f8e9cbd199b8b4930bb4763c4784dec90a87a3`  
		Last Modified: Tue, 02 Aug 2022 13:23:26 GMT  
		Size: 156.4 MB (156437369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eababc8c7c81e20c686147ea76b329aa1241aea64cdbc651f4bf66b21854053`  
		Last Modified: Wed, 03 Aug 2022 00:07:12 GMT  
		Size: 23.4 MB (23394454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf81eccc910d35f336f1e02f1d6a250a4f993d1d37da878cb043600a0ed1aa0`  
		Last Modified: Wed, 03 Aug 2022 00:07:10 GMT  
		Size: 8.7 MB (8739490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3f8b7aaf22ecf6cf504bbc72c3aadc18f95e4f3b2d50d5b7e9656aef722541`  
		Last Modified: Wed, 03 Aug 2022 00:07:10 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5176559d6699f79b36269d3ccbc3ebea74f8d924e93366f1f600a5960315990`  
		Last Modified: Wed, 03 Aug 2022 00:07:10 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
