## `maven:3-ibmjava`

```console
$ docker pull maven@sha256:9f70f36f5c9b903acb9d814f4755ee00978cb41f2559eafda6614eed151e84d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-ibmjava` - linux; amd64

```console
$ docker pull maven@sha256:3027a479d3b036a2802a594f63fc7d39eac1b40259c7f34aaf560db58664ab30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.7 MB (235725608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:612877a370271145bbab59101cd76746817d17f54a6ca969c2664fddef1ada08`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:19:05 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 13 Jul 2021 23:19:13 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:19:14 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Tue, 13 Jul 2021 23:21:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ebb0fd9e7e49b541663ea152a4c28b4d85c458fb00a35e407bfd922fea418fae';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dcf59f47f74e6ab9b9b1b36f17f31ce9ae800a54d3f8911ee4380a5f128071d7';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='124006e81d5fb148face2142ff7b6155c62876c6f819844d2d34d8d174a0efe7';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='46e8263da8b7cd80b780f5a9dbdab4f0000c32907af1ecbfe58edfc3068810e7';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='73fb5069d838eeeecbb801c4a8a03180a96e724dad79ef1b441be36ee8d53195';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 13 Jul 2021 23:21:22 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 14 Jul 2021 03:48:28 GMT
ARG MAVEN_VERSION=3.8.1
# Wed, 14 Jul 2021 03:48:28 GMT
ARG USER_HOME_DIR=/root
# Wed, 14 Jul 2021 03:48:29 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Wed, 14 Jul 2021 03:48:29 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Wed, 14 Jul 2021 03:48:48 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 14 Jul 2021 03:48:48 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 14 Jul 2021 03:48:49 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 14 Jul 2021 03:48:49 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 14 Jul 2021 03:48:50 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 14 Jul 2021 03:48:50 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 14 Jul 2021 03:48:50 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22821a14390caaab5b1f7ca9feb8e54ce64d3d81ca1fa64c6f1eee32ae92da5b`  
		Last Modified: Tue, 13 Jul 2021 23:23:03 GMT  
		Size: 3.0 MB (2959004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b90295c40970bbb17ff1570addc7017c9b85451a44f5e27176685bcda6cf7bf5`  
		Last Modified: Tue, 13 Jul 2021 23:23:59 GMT  
		Size: 166.7 MB (166681009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022c81c5d21a4b381e3cb68f9ce41abeeff3cf210e8217622041f5b01de1fb3b`  
		Last Modified: Wed, 14 Jul 2021 03:56:28 GMT  
		Size: 39.4 MB (39378236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afec7311d4fffbb39aec5774f1dd30ee8a248856016ee8b649d065ceb3c66901`  
		Last Modified: Wed, 14 Jul 2021 03:56:24 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f5388611d8bb1fd1653f2c1c21802da889be7e2daf7b3f2a8092fd18692f8b`  
		Last Modified: Wed, 14 Jul 2021 03:56:24 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibmjava` - linux; 386

```console
$ docker pull maven@sha256:14f274b7771aa16f211e55bb9781ad3c51225df0f4f758b2b41e997a48e5db94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (221980153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82012f250afd42ea0ff45db58612695c3ab285bc6d816b0c31913c97fe4596a1`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 13 Jul 2021 22:39:15 GMT
ADD file:2478887c0caae58ac755f71306211decbf5e69b832b9939974a93743e5c440f5 in / 
# Tue, 13 Jul 2021 22:39:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:05:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 13 Jul 2021 23:05:35 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:05:35 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Tue, 13 Jul 2021 23:07:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ebb0fd9e7e49b541663ea152a4c28b4d85c458fb00a35e407bfd922fea418fae';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dcf59f47f74e6ab9b9b1b36f17f31ce9ae800a54d3f8911ee4380a5f128071d7';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='124006e81d5fb148face2142ff7b6155c62876c6f819844d2d34d8d174a0efe7';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='46e8263da8b7cd80b780f5a9dbdab4f0000c32907af1ecbfe58edfc3068810e7';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='73fb5069d838eeeecbb801c4a8a03180a96e724dad79ef1b441be36ee8d53195';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 13 Jul 2021 23:07:55 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Tue, 13 Jul 2021 23:48:07 GMT
ARG MAVEN_VERSION=3.8.1
# Tue, 13 Jul 2021 23:48:07 GMT
ARG USER_HOME_DIR=/root
# Tue, 13 Jul 2021 23:48:07 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Tue, 13 Jul 2021 23:48:08 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Tue, 13 Jul 2021 23:48:45 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 13 Jul 2021 23:48:45 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 13 Jul 2021 23:48:46 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 13 Jul 2021 23:48:46 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 13 Jul 2021 23:48:46 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 13 Jul 2021 23:48:46 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 13 Jul 2021 23:48:47 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:4c0067b0d84ac31443135f34e6bf8eacb1e1da0b388d042fbdd498858738047f`  
		Last Modified: Tue, 13 Jul 2021 22:40:10 GMT  
		Size: 27.2 MB (27153547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbe1128ef2eac594ca8c851354f334bde2c6c46096bbce3775054be4560ce98`  
		Last Modified: Tue, 13 Jul 2021 23:08:30 GMT  
		Size: 3.0 MB (2988008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537c0e8e38af1c8a98d2d59ecc6e896e11d7e64e6c7066c66282ec2de913d704`  
		Last Modified: Tue, 13 Jul 2021 23:09:34 GMT  
		Size: 154.7 MB (154746848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8362f1d870c9f9a0cd2995957e1d403ed7857d2654b9639d04f0c63eb7a99ff1`  
		Last Modified: Tue, 13 Jul 2021 23:49:23 GMT  
		Size: 37.1 MB (37090536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707c4f12f2aa4fbda1935dbaaf54b41a5537bef689f62c3a23d2513e34e9832`  
		Last Modified: Tue, 13 Jul 2021 23:49:18 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9110a4af97d0ee5420a2e9cce7eae5aefc75718f1ef9711ac123d0519a93b71`  
		Last Modified: Tue, 13 Jul 2021 23:49:18 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibmjava` - linux; ppc64le

```console
$ docker pull maven@sha256:9c75c57229d1c589fc9f4aca743c8a8b121459e9505a68b397f43defdff15105
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234332167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508c3c99089a4d4c5adbb4d06c01b68c2ef7439ed8131e3b55609f61959b8cf3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:01:35 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 02:02:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:02:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 02:07:02 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ebb0fd9e7e49b541663ea152a4c28b4d85c458fb00a35e407bfd922fea418fae';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dcf59f47f74e6ab9b9b1b36f17f31ce9ae800a54d3f8911ee4380a5f128071d7';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='124006e81d5fb148face2142ff7b6155c62876c6f819844d2d34d8d174a0efe7';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='46e8263da8b7cd80b780f5a9dbdab4f0000c32907af1ecbfe58edfc3068810e7';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='73fb5069d838eeeecbb801c4a8a03180a96e724dad79ef1b441be36ee8d53195';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 02:07:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 18 Jun 2021 04:44:45 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 18 Jun 2021 04:44:49 GMT
ARG USER_HOME_DIR=/root
# Fri, 18 Jun 2021 04:44:52 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 18 Jun 2021 04:44:58 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 18 Jun 2021 04:46:40 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 18 Jun 2021 04:46:50 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 18 Jun 2021 04:46:57 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 18 Jun 2021 04:46:58 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 18 Jun 2021 04:47:00 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 18 Jun 2021 04:47:04 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 18 Jun 2021 04:47:09 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8d177e4917900437a3445272639bed389b718cc65a87346ba94f6d99327f34`  
		Last Modified: Fri, 18 Jun 2021 02:07:44 GMT  
		Size: 3.1 MB (3082963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506461e1b2a40e239b8941766feecc9bf40ee6e3a6928b14c3c4e5bf2bc9a0d9`  
		Last Modified: Fri, 18 Jun 2021 02:08:51 GMT  
		Size: 166.3 MB (166338694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ba0e8c8d5507824a6e2be4f7a47a1e32b4918e86f642d7c3317ae5936daedf`  
		Last Modified: Fri, 18 Jun 2021 04:50:58 GMT  
		Size: 34.5 MB (34483940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd955233b1d816508ead264ce50bd3a7e54fae1f8f0988ac5facc0b2d3b1c88a`  
		Last Modified: Fri, 18 Jun 2021 04:50:54 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671581f358f2b7acf86b1d5978ed5ee17cc9f9489bae44bd61e08d9dc803895d`  
		Last Modified: Fri, 18 Jun 2021 04:50:54 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibmjava` - linux; s390x

```console
$ docker pull maven@sha256:6f7c85c59b31fd81ce1ae5da72e8df3dab94a98c571f740e780c5567539f24d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217528902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85aaa4ea7a6930776f889c78519bd0fa0db4217c79b9d40c65f624ddd0437d5e`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 13 Jul 2021 22:53:22 GMT
ADD file:9e621b1dfa735f1a89553f154f2a2a6f669ff610236d92d6ebf37d1f378d8ec0 in / 
# Tue, 13 Jul 2021 22:53:24 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:12:13 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 13 Jul 2021 23:12:20 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:12:20 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Tue, 13 Jul 2021 23:14:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ebb0fd9e7e49b541663ea152a4c28b4d85c458fb00a35e407bfd922fea418fae';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dcf59f47f74e6ab9b9b1b36f17f31ce9ae800a54d3f8911ee4380a5f128071d7';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='124006e81d5fb148face2142ff7b6155c62876c6f819844d2d34d8d174a0efe7';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='46e8263da8b7cd80b780f5a9dbdab4f0000c32907af1ecbfe58edfc3068810e7';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='73fb5069d838eeeecbb801c4a8a03180a96e724dad79ef1b441be36ee8d53195';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 13 Jul 2021 23:14:52 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 14 Jul 2021 00:20:30 GMT
ARG MAVEN_VERSION=3.8.1
# Wed, 14 Jul 2021 00:20:31 GMT
ARG USER_HOME_DIR=/root
# Wed, 14 Jul 2021 00:20:31 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Wed, 14 Jul 2021 00:20:32 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Wed, 14 Jul 2021 00:20:54 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 14 Jul 2021 00:20:55 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 14 Jul 2021 00:20:56 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 14 Jul 2021 00:20:56 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 14 Jul 2021 00:20:56 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 14 Jul 2021 00:20:56 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 14 Jul 2021 00:20:57 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3287e09e36098b10234ccc1f8db0b48e2027ca7caa353a362d65f9b017ab802e`  
		Last Modified: Tue, 13 Jul 2021 22:55:34 GMT  
		Size: 25.4 MB (25365649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6fe4e2b151f33398a6ef48bbb5d9ace538aa5ecf3fab9182babc3a85b9166b`  
		Last Modified: Tue, 13 Jul 2021 23:16:59 GMT  
		Size: 2.7 MB (2676828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e107d093f0ddb6173da707d07364554373c98b1e6f85874cd83d11687d60ac1c`  
		Last Modified: Tue, 13 Jul 2021 23:17:43 GMT  
		Size: 157.0 MB (156959462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8811d5361f7ce907a3b821fb3bc3a37fa86411ba70d9adb7ba90c7a9436682`  
		Last Modified: Wed, 14 Jul 2021 00:24:55 GMT  
		Size: 32.5 MB (32525749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2812696f81fff72d2d905e9270684f545cb3de893ef56902b1ec756c0af7c54`  
		Last Modified: Wed, 14 Jul 2021 00:24:53 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6bd7c5875912712ce0dfd842963ae14306e76706492ce789362cf79b919fff`  
		Last Modified: Wed, 14 Jul 2021 00:24:53 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
