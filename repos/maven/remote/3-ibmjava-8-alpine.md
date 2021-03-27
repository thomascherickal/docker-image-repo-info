## `maven:3-ibmjava-8-alpine`

```console
$ docker pull maven@sha256:98958ca87edf8718176bd9b7b5548fcbb812517d926cf08ff94103c899298a22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `maven:3-ibmjava-8-alpine` - linux; amd64

```console
$ docker pull maven@sha256:9045c93df4ddc41a9de93eef5a3d1f184a3c9c7fae631e1b1cb1d7bdd14b6117
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.6 MB (187608336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcb86e6b259464068fef7366f3c9e4e9e220e74d5ebe03ba73393d05ae357689`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:31:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 09:31:54 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Fri, 26 Mar 2021 09:32:04 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Fri, 26 Mar 2021 09:32:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 09:35:21 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='c51b7afed4911a4eefdf02c44ee440de726a5a605c5507cc50d4795394b418c2';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dfe87d34c40cd0c23dc4b7ee47c85f84e26d21ff75476b234998bb9132379659';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='bbc55934ec867290cd9307422beae48e5032dfabb7cb496bed6e47b7ab3f90be';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ed2722f283a3f3eb0a71f23354b0b4d2761865e759a3bf7f89297e17c20e6f';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='c2ddf185daafacd0b50f3e4e593d613b2e9b70d66b88a8da6ee313181376aef6';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Fri, 26 Mar 2021 09:35:22 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 19:00:29 GMT
RUN apk add --no-cache curl tar bash procps
# Fri, 26 Mar 2021 19:00:29 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 26 Mar 2021 19:00:29 GMT
ARG USER_HOME_DIR=/root
# Fri, 26 Mar 2021 19:00:30 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 26 Mar 2021 19:00:30 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 26 Mar 2021 19:00:32 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 26 Mar 2021 19:00:32 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 26 Mar 2021 19:00:33 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 26 Mar 2021 19:00:33 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 26 Mar 2021 19:00:33 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 26 Mar 2021 19:00:33 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 26 Mar 2021 19:00:33 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdada4ef0dc073217b626a0e26cb68e2f8bf5a887558a89825a167331bcbe09`  
		Last Modified: Fri, 26 Mar 2021 09:36:17 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b6877caf7aeef3d80a1d0f5f907e7ead88685e5f791be0a70530a1e4c63c26`  
		Last Modified: Fri, 26 Mar 2021 09:36:18 GMT  
		Size: 5.5 MB (5539753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd824891f5203d789e1ecb7fa9ed26f1e6bb9299e145bae2c8fb710b570c49c`  
		Last Modified: Fri, 26 Mar 2021 09:37:47 GMT  
		Size: 168.0 MB (168007845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd89916e173c77862d1f1dd8daf9bd6f8ef91d421ec2587eed49aa799a86802d`  
		Last Modified: Fri, 26 Mar 2021 19:07:33 GMT  
		Size: 1.7 MB (1678025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1232f5297c07228c55b0773ac59f38e255f6690067a9a13d6aa97e3ca29afc`  
		Last Modified: Fri, 26 Mar 2021 19:07:34 GMT  
		Size: 9.6 MB (9581198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f585100c8af0b358416a2ba70ecd01c515bdd26ee90f587aa9cc98ab230261e2`  
		Last Modified: Fri, 26 Mar 2021 19:07:32 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c247e1d42c7a868d77c50a736c4c979d634da87776aa45bd59c9a7e5d38bce`  
		Last Modified: Fri, 26 Mar 2021 19:07:33 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
