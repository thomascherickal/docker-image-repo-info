## `ibmjava:8-sdk`

```console
$ docker pull ibmjava@sha256:1e24a03d9e62f1ed0a868be2b3572b0286633c291eb5f6f299f73dd3a1805c1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:fa52c51c364e5e94b769f757cbce8d1bb350064b2ebf7d688a3effb01604a0b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196139045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a6261a03fcd5ccfd1284cbc51a0e996c2ae3da8e259f1595df2a2d197a17aa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:33:47 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 02 Mar 2023 04:33:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:33:55 GMT
ENV JAVA_VERSION=8.0.7.20
# Thu, 02 Mar 2023 04:36:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='0f6aef4c3550a8f85288da8bc6fada405b0ce2226d6b1b57d0aae98cd5eef5e4';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='fa7661c2eb2982c4fb85c6894e7a975970b27b6ee82d5facb352f075cc1dfca3';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a56803671fe7d1c85f18d566dbcb7fbaf1d60c6f1d6de34e35a257e0c8095f9b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='71c913a1eed7daae952657e18eb9a2e71723106b6e7b56373f18564db77f551e';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='c8641bc22443ebccaedf1822a12ec1303d89577d45c875702e1f628066c7f383';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 02 Mar 2023 04:36:55 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4584491976e0a2288553243d3caf1fc9a32b4827c131397e78d378040794a302`  
		Last Modified: Thu, 02 Mar 2023 04:37:19 GMT  
		Size: 3.0 MB (2952434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e80434905a67b8436af9db87a072f9e63fdccce65f0c273baafb2cc459457f`  
		Last Modified: Thu, 02 Mar 2023 04:38:06 GMT  
		Size: 166.5 MB (166475458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:e7937c6f989c3344a9d1e0c5f9fedc905d9f5c0f55ae1f5859e94bc1c0939f64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.6 MB (184641524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601eaa609e2faa044927d641ac898d86799eddd82379e89728369ef6b8f6c14a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:01 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:03 GMT
ADD file:b9b814a7d1e7611a2c531fac3419a48c733c622470d3f275ce29f9ba8764eaeb in / 
# Thu, 26 Jan 2023 10:03:04 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:43:13 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Jan 2023 17:43:20 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:43:20 GMT
ENV JAVA_VERSION=8.0.7.20
# Tue, 31 Jan 2023 17:47:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='0f6aef4c3550a8f85288da8bc6fada405b0ce2226d6b1b57d0aae98cd5eef5e4';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='fa7661c2eb2982c4fb85c6894e7a975970b27b6ee82d5facb352f075cc1dfca3';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a56803671fe7d1c85f18d566dbcb7fbaf1d60c6f1d6de34e35a257e0c8095f9b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='71c913a1eed7daae952657e18eb9a2e71723106b6e7b56373f18564db77f551e';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='c8641bc22443ebccaedf1822a12ec1303d89577d45c875702e1f628066c7f383';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Jan 2023 17:47:05 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:a1177ecacc42e51782037ed649a91241b82866cc72c6eb0f205cbcc350f44d43`  
		Last Modified: Tue, 31 Jan 2023 17:42:04 GMT  
		Size: 27.2 MB (27165349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bd4ed927791f68d34f96a84af2a713efcb2234c018146289b0a0fafb33eef2`  
		Last Modified: Tue, 31 Jan 2023 17:47:42 GMT  
		Size: 3.0 MB (2981539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c37f7c0b2f224cfbbe89118e9dd236eecff6987c8848732440d0dc1fdbb4f7`  
		Last Modified: Tue, 31 Jan 2023 17:48:41 GMT  
		Size: 154.5 MB (154494636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:93df3681713df27d21976be79f9be35eefb88d7ab280a897240e1b60bb0597b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.8 MB (199791366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ef7ffe0941203680fb2744450bbba2250faf5897d4a132720ffe995ce44948`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:15:24 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:15:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:15:27 GMT
ADD file:ca5a453351fddb6d7937e334f0331321829a5bebca3d726ef3dddad1f23b35c8 in / 
# Wed, 01 Mar 2023 03:15:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:26:13 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 02 Mar 2023 04:26:46 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:26:47 GMT
ENV JAVA_VERSION=8.0.7.20
# Thu, 02 Mar 2023 04:33:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='0f6aef4c3550a8f85288da8bc6fada405b0ce2226d6b1b57d0aae98cd5eef5e4';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='fa7661c2eb2982c4fb85c6894e7a975970b27b6ee82d5facb352f075cc1dfca3';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a56803671fe7d1c85f18d566dbcb7fbaf1d60c6f1d6de34e35a257e0c8095f9b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='71c913a1eed7daae952657e18eb9a2e71723106b6e7b56373f18564db77f551e';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='c8641bc22443ebccaedf1822a12ec1303d89577d45c875702e1f628066c7f383';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 02 Mar 2023 04:33:57 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:27fbc2bd86045e72ba8d9901b237295e3094b37f456824337175e24a0f0afe98`  
		Last Modified: Thu, 02 Mar 2023 03:09:44 GMT  
		Size: 30.4 MB (30442026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ba0371be9483ee0b28a477686cea779ddaceb8d8bac7c4e6fe24bf77052c7e`  
		Last Modified: Thu, 02 Mar 2023 04:34:32 GMT  
		Size: 3.1 MB (3077279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079acaa024811784dc99b555e6c85be46967249aa8d08a692efd3aa71645a852`  
		Last Modified: Thu, 02 Mar 2023 04:35:43 GMT  
		Size: 166.3 MB (166272061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:90e85adeb1522f5cbcc2f9319494532d95f8f9c5935942b20e8d88314338d0de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.8 MB (184804744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b79d2fe5ac5614d0be3f633b9a34b90bf148e5e323fd32401f7d771639622fd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:09 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:11 GMT
ADD file:49b5368b8703fe0aa128fe923b83da7ab2a30a7a1c0395682c905b9271e7f503 in / 
# Wed, 01 Mar 2023 03:18:11 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:01:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 02 Mar 2023 03:01:59 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:02:00 GMT
ENV JAVA_VERSION=8.0.7.20
# Thu, 02 Mar 2023 03:04:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='0f6aef4c3550a8f85288da8bc6fada405b0ce2226d6b1b57d0aae98cd5eef5e4';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='fa7661c2eb2982c4fb85c6894e7a975970b27b6ee82d5facb352f075cc1dfca3';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a56803671fe7d1c85f18d566dbcb7fbaf1d60c6f1d6de34e35a257e0c8095f9b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='71c913a1eed7daae952657e18eb9a2e71723106b6e7b56373f18564db77f551e';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='c8641bc22443ebccaedf1822a12ec1303d89577d45c875702e1f628066c7f383';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 02 Mar 2023 03:04:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:306d1b363f89f239f5dc6314e0033094c067617b584ce004fd8db99402dab321`  
		Last Modified: Thu, 02 Mar 2023 02:21:31 GMT  
		Size: 25.4 MB (25371412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fe795fb99ed72a95436de37d2cdb8fbd2edb3445e421c880c502757fb41be9`  
		Last Modified: Thu, 02 Mar 2023 03:05:21 GMT  
		Size: 2.7 MB (2669070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1faca277882f5361876339ebbf10a447709eb207e81aea404f21a9db495ec02`  
		Last Modified: Thu, 02 Mar 2023 03:06:04 GMT  
		Size: 156.8 MB (156764262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
