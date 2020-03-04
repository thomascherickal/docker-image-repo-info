## `ibmjava:jre-alpine`

```console
$ docker pull ibmjava@sha256:816fc68890769407dfc57e4ce55c93964e083a4f66ff98b283116dcd39ee1a31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:jre-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:aa6f6e772171c5f0116b9a87a4debb490d793baa173ce38c70e75462b0d961cf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138631800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9b3d1fd4dd3e5413218308255596cc5a297c69a80696304334de8f298eb4ca7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 18:58:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 23 Jan 2020 18:58:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Thu, 23 Jan 2020 18:58:26 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Wed, 04 Mar 2020 02:20:27 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Wed, 04 Mar 2020 02:21:07 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Wed, 04 Mar 2020 02:21:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dae0f47127209aea70646977ebe366124ed65f82542cf651f109356bff110b`  
		Last Modified: Thu, 23 Jan 2020 19:01:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fad1ca64c34cb5644888bf2c8ae8fee9a4b1c9437b10bf8c0242dc13ce232a`  
		Last Modified: Thu, 23 Jan 2020 19:01:33 GMT  
		Size: 5.6 MB (5565608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969f86d3702b0977ae457161bd57a4b98b528f43368998271674e5484dc0d811`  
		Last Modified: Wed, 04 Mar 2020 02:25:06 GMT  
		Size: 130.3 MB (130278685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
