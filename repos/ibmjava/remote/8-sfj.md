## `ibmjava:8-sfj`

```console
$ docker pull ibmjava@sha256:f5171b45b926f850e9e31e0b9cd882f9f0c28bf387cf2d5798e89e74c4a93b45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:7d22a0f237b59c643460d43e4defee3e8b549f0a06a3287324b945c7d2d24cf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94536396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21176977374beb1433a858ab721a0083ceadad531a120e6d614cf26cd0cdc037`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:52:33 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 02:52:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:19:40 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:21:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='68d93db98bfde238b8a53089a2e89eb9927ae7a46dc2a20e41a1655e882ebe18';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='5732b958332885e1bea39105018ac23297bc871ba78c29ce92b208ed87967b17';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c3f53130efb66f541aa0492c471187176d2eb5cbb6aa12ae8ddbdc818de28e9a';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e06fe432da13c9e5fd082f9d16f59d7d7f0198a819393f392bc9b1f08050fb20';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='3e3a577a8322001d73fde8144f7a7a9400f73bc0e709f8057ece0432386143b1';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:21:49 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:dbb50312bb188587b317baf2ac44e706adaaf57db35020164ba44ac57194b4af`  
		Last Modified: Wed, 29 Jun 2022 18:23:51 GMT  
		Size: 64.9 MB (64864550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:6053ccdc1f3e1fee803a613353d944c575445d32a467c528632ea9b7fd581e3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94408936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2931f87b32a51a39bdd4f9714f49f18faf92b3bc3a6e7b7f0cbeeb8d94eeaffd`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 21:18:54 GMT
ADD file:c1118975f50d6835777043d4b807b4fcf30db0151d1e7659e077e9e33c4ea7c7 in / 
# Mon, 06 Jun 2022 21:18:54 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 21:52:30 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 06 Jun 2022 21:52:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:38:35 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:40:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='68d93db98bfde238b8a53089a2e89eb9927ae7a46dc2a20e41a1655e882ebe18';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='5732b958332885e1bea39105018ac23297bc871ba78c29ce92b208ed87967b17';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c3f53130efb66f541aa0492c471187176d2eb5cbb6aa12ae8ddbdc818de28e9a';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e06fe432da13c9e5fd082f9d16f59d7d7f0198a819393f392bc9b1f08050fb20';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='3e3a577a8322001d73fde8144f7a7a9400f73bc0e709f8057ece0432386143b1';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:40:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:1408ae6e2634d0ef0a2f110363deef0fdf35ee2958852f9d20b92b57495a9fb7`  
		Last Modified: Mon, 06 Jun 2022 21:19:41 GMT  
		Size: 27.2 MB (27165461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2544d5d24f04fcdb404016e3858b5878b2ee1182436bb2acb9f0b694ad952bb2`  
		Last Modified: Mon, 06 Jun 2022 21:55:15 GMT  
		Size: 3.0 MB (2989000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed80a15b8ba4c18c4d9372be04a450b4c6ee22f4ed7c721d0f680ef94d1f5dc`  
		Last Modified: Wed, 29 Jun 2022 18:42:50 GMT  
		Size: 64.3 MB (64254475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:d4b8cfa680cff00ef0e3cb37352d2588f8c0623d0bb4f9ca0dd67e1b2b8949cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.5 MB (98531004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99124ed7fb73966e461efadcd97d67cc1879dacb97a307c85c573679cd80b9ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:49:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 08:50:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:31:53 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:34:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='68d93db98bfde238b8a53089a2e89eb9927ae7a46dc2a20e41a1655e882ebe18';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='5732b958332885e1bea39105018ac23297bc871ba78c29ce92b208ed87967b17';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c3f53130efb66f541aa0492c471187176d2eb5cbb6aa12ae8ddbdc818de28e9a';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e06fe432da13c9e5fd082f9d16f59d7d7f0198a819393f392bc9b1f08050fb20';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='3e3a577a8322001d73fde8144f7a7a9400f73bc0e709f8057ece0432386143b1';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:34:53 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4a22aedc3b9f2593635b0a3f6fe64e6dd424850b9782f66e88c8c162926d6a`  
		Last Modified: Tue, 07 Jun 2022 08:54:16 GMT  
		Size: 3.1 MB (3082521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e59e0466e208ba61404e5721ccaa64db3ba41a273e9436234e7c2ad486f0a4`  
		Last Modified: Wed, 29 Jun 2022 18:38:29 GMT  
		Size: 65.0 MB (65005624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:a0023333ccce0409ad773fb3d469ab7a1a935411c004f116d8da5ce2cf2b41f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (93970858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a689ec6fd156bb0185b12c18fefc500d17de3e7adf54cb651600e3ed49ff7b34`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 04:04:44 GMT
ADD file:e2caa30d22701eeadebe1abd66923745f75d170d7baa51a62119576c31b7f89c in / 
# Tue, 07 Jun 2022 04:04:47 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:27:04 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 06:27:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:41:46 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:44:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='68d93db98bfde238b8a53089a2e89eb9927ae7a46dc2a20e41a1655e882ebe18';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='5732b958332885e1bea39105018ac23297bc871ba78c29ce92b208ed87967b17';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c3f53130efb66f541aa0492c471187176d2eb5cbb6aa12ae8ddbdc818de28e9a';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e06fe432da13c9e5fd082f9d16f59d7d7f0198a819393f392bc9b1f08050fb20';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='3e3a577a8322001d73fde8144f7a7a9400f73bc0e709f8057ece0432386143b1';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:44:34 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:e783523fdb31436e9a84774bee5bba6b8d49250e29b4110742d8bfcbb1b69556`  
		Last Modified: Wed, 29 Jun 2022 18:47:03 GMT  
		Size: 65.9 MB (65923259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
