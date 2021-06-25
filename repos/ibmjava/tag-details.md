<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ibmjava`

-	[`ibmjava:11`](#ibmjava11)
-	[`ibmjava:11-jdk`](#ibmjava11-jdk)
-	[`ibmjava:8`](#ibmjava8)
-	[`ibmjava:8-jre`](#ibmjava8-jre)
-	[`ibmjava:8-jre-alpine`](#ibmjava8-jre-alpine)
-	[`ibmjava:8-sdk`](#ibmjava8-sdk)
-	[`ibmjava:8-sdk-alpine`](#ibmjava8-sdk-alpine)
-	[`ibmjava:8-sfj`](#ibmjava8-sfj)
-	[`ibmjava:8-sfj-alpine`](#ibmjava8-sfj-alpine)
-	[`ibmjava:jre`](#ibmjavajre)
-	[`ibmjava:jre-alpine`](#ibmjavajre-alpine)
-	[`ibmjava:latest`](#ibmjavalatest)
-	[`ibmjava:sdk`](#ibmjavasdk)
-	[`ibmjava:sdk-alpine`](#ibmjavasdk-alpine)
-	[`ibmjava:sfj`](#ibmjavasfj)
-	[`ibmjava:sfj-alpine`](#ibmjavasfj-alpine)

## `ibmjava:11`

```console
$ docker pull ibmjava@sha256:a9d2c576019ce8612b7b8c4fcceeba5bf813a9e685b776ac9cff85b1bebc6527
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:11` - linux; amd64

```console
$ docker pull ibmjava@sha256:b0444624f68aa0a92c421b86b09e0e88534606fa656e75284f35f29a0857ece2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.0 MB (261970805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0c2434ebddeba9c874a7ccbac6756dcd740f526694a2c4ef9a42a6c5e2168f9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 08:41:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 24 Jun 2021 08:41:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 08:41:41 GMT
ENV JAVA_VERSION=11.0.11.0
# Thu, 24 Jun 2021 08:42:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 24 Jun 2021 08:42:37 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bf810f87ab47830bc958342a7c302326b7dd180c426bb4f24a55e815c4691e`  
		Last Modified: Thu, 24 Jun 2021 08:43:11 GMT  
		Size: 3.0 MB (3038988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba6dfe965b3c1caeaec650a51807aac4b120e6a4e988dd7b41ffcb8bf4bf2fc`  
		Last Modified: Thu, 24 Jun 2021 08:43:29 GMT  
		Size: 230.4 MB (230378125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:11` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:f29c19cc5de8b5334916d16369e7d2d662a952d8b3bed87532da00b2f12cc57e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.9 MB (267876276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea1e896f3498d265d3190991606e6988e7be71257e02b719b790d920adf70d9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 17:24:01 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 24 Jun 2021 17:24:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 17:24:57 GMT
ENV JAVA_VERSION=11.0.11.0
# Thu, 24 Jun 2021 17:26:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 24 Jun 2021 17:26:25 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7345e9b987bf8fc71a025de52cb59ade60aa62853c8a2d637b7ea84bc7903`  
		Last Modified: Thu, 24 Jun 2021 17:26:58 GMT  
		Size: 3.3 MB (3292475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1202be7f2929f9707ee69ce78d1d578693cab0e27ba6a516fb20ce304c31d97`  
		Last Modified: Thu, 24 Jun 2021 17:27:25 GMT  
		Size: 231.3 MB (231305556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:11` - linux; s390x

```console
$ docker pull ibmjava@sha256:2054ee2b1728f46b7c37e02518aeb0ae427205fe4284958b2674dc8549a6b045
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.6 MB (258585871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e42746d35cf216a4e65badb28fc4ad07cef0742c102a7725dbe8208369316ee7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:44:00 GMT
ADD file:737a08bab262cc2abc326912fdb8c8038222b272a5967b25ec6c761539c9d456 in / 
# Thu, 17 Jun 2021 23:44:02 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 19:41:56 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 23 Jun 2021 19:42:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 19:42:03 GMT
ENV JAVA_VERSION=11.0.11.0
# Wed, 23 Jun 2021 19:43:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 23 Jun 2021 19:43:10 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:be436b7e641e3737311249dadcc71ad61ba7bc9597248f426c58c8548cff8af0`  
		Last Modified: Thu, 17 Jun 2021 23:45:32 GMT  
		Size: 27.1 MB (27140902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c53126120716f101dab95f63591f1b4a63b9ede45db77e0d39b5b77acdc44b`  
		Last Modified: Wed, 23 Jun 2021 19:43:30 GMT  
		Size: 2.7 MB (2737598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47bfe568f02668782f796d670c090162adf2a35c786e09d9a5fcc40df3415b`  
		Last Modified: Wed, 23 Jun 2021 19:43:45 GMT  
		Size: 228.7 MB (228707371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:11-jdk`

```console
$ docker pull ibmjava@sha256:a9d2c576019ce8612b7b8c4fcceeba5bf813a9e685b776ac9cff85b1bebc6527
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:11-jdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:b0444624f68aa0a92c421b86b09e0e88534606fa656e75284f35f29a0857ece2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.0 MB (261970805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0c2434ebddeba9c874a7ccbac6756dcd740f526694a2c4ef9a42a6c5e2168f9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 08:41:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 24 Jun 2021 08:41:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 08:41:41 GMT
ENV JAVA_VERSION=11.0.11.0
# Thu, 24 Jun 2021 08:42:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 24 Jun 2021 08:42:37 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bf810f87ab47830bc958342a7c302326b7dd180c426bb4f24a55e815c4691e`  
		Last Modified: Thu, 24 Jun 2021 08:43:11 GMT  
		Size: 3.0 MB (3038988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba6dfe965b3c1caeaec650a51807aac4b120e6a4e988dd7b41ffcb8bf4bf2fc`  
		Last Modified: Thu, 24 Jun 2021 08:43:29 GMT  
		Size: 230.4 MB (230378125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:11-jdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:f29c19cc5de8b5334916d16369e7d2d662a952d8b3bed87532da00b2f12cc57e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.9 MB (267876276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea1e896f3498d265d3190991606e6988e7be71257e02b719b790d920adf70d9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 17:24:01 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 24 Jun 2021 17:24:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 17:24:57 GMT
ENV JAVA_VERSION=11.0.11.0
# Thu, 24 Jun 2021 17:26:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 24 Jun 2021 17:26:25 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7345e9b987bf8fc71a025de52cb59ade60aa62853c8a2d637b7ea84bc7903`  
		Last Modified: Thu, 24 Jun 2021 17:26:58 GMT  
		Size: 3.3 MB (3292475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1202be7f2929f9707ee69ce78d1d578693cab0e27ba6a516fb20ce304c31d97`  
		Last Modified: Thu, 24 Jun 2021 17:27:25 GMT  
		Size: 231.3 MB (231305556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:11-jdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:2054ee2b1728f46b7c37e02518aeb0ae427205fe4284958b2674dc8549a6b045
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.6 MB (258585871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e42746d35cf216a4e65badb28fc4ad07cef0742c102a7725dbe8208369316ee7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:44:00 GMT
ADD file:737a08bab262cc2abc326912fdb8c8038222b272a5967b25ec6c761539c9d456 in / 
# Thu, 17 Jun 2021 23:44:02 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 19:41:56 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 23 Jun 2021 19:42:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 19:42:03 GMT
ENV JAVA_VERSION=11.0.11.0
# Wed, 23 Jun 2021 19:43:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 23 Jun 2021 19:43:10 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:be436b7e641e3737311249dadcc71ad61ba7bc9597248f426c58c8548cff8af0`  
		Last Modified: Thu, 17 Jun 2021 23:45:32 GMT  
		Size: 27.1 MB (27140902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c53126120716f101dab95f63591f1b4a63b9ede45db77e0d39b5b77acdc44b`  
		Last Modified: Wed, 23 Jun 2021 19:43:30 GMT  
		Size: 2.7 MB (2737598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47bfe568f02668782f796d670c090162adf2a35c786e09d9a5fcc40df3415b`  
		Last Modified: Wed, 23 Jun 2021 19:43:45 GMT  
		Size: 228.7 MB (228707371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8`

```console
$ docker pull ibmjava@sha256:2c15590702d6a77ffa99a34f0c96a8bd7fd4f5a8248067564b7d5e15c26e719d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8` - linux; amd64

```console
$ docker pull ibmjava@sha256:57b1e6a944d9e2946516fc102d45d45e9d970a89b94963503f4c16324bafb2d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.2 MB (159196341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88d22d1bd2ef5ecabe40773943bc721e0c4500375984bb33d941198da6e836a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:26:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 01:26:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:26:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 01:27:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 01:27:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff3851d5fd9b952f0838f935196e2af17f7b597965441e75928bd4a7c7fda14`  
		Last Modified: Fri, 18 Jun 2021 01:29:04 GMT  
		Size: 3.0 MB (2959474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501e9b2fcdbe46c416058775ecae3071cb3a5182dfb4747ecb6775ea313b6b22`  
		Last Modified: Fri, 18 Jun 2021 01:29:13 GMT  
		Size: 129.5 MB (129536161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8` - linux; 386

```console
$ docker pull ibmjava@sha256:66e66e06954ce313b3d6295eff2a0a8825f4f4de3e09d77b454be4a0b1b5aa56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147864344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb4dd151fcd34a2577fdc78b167711bee47aa2d0e521ce92c47c1cd22b05cc3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:47:53 GMT
ADD file:3065820b37abf9a8ea82d39405ed55dc52d1e1ae7591a0a9d1c8a64e7287e06d in / 
# Thu, 17 Jun 2021 23:47:54 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:20:56 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:21:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:21:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:21:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:21:41 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:f76fac8c74a781007cb52b5223c59c8f3908bc41ecf0ae8f6dc9046b0aa24e58`  
		Last Modified: Thu, 17 Jun 2021 23:48:46 GMT  
		Size: 27.1 MB (27146196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5384f13a1fdaed1da8671f29859baba07658d2cb4ebdc38e420afb1856bb66`  
		Last Modified: Fri, 18 Jun 2021 00:23:42 GMT  
		Size: 3.0 MB (2987983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e0d59c7eca714b5a641beceded38d52ca85d0d9c6248bcfef384791113cc43`  
		Last Modified: Fri, 18 Jun 2021 00:23:54 GMT  
		Size: 117.7 MB (117730165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:5b9acd7af8fd6f362c2d1e28666902aa815df5241ec8a0e43f36a8b5091fc561
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162568110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589254cf8583fa55985ef5cd52338ffb045060ffae67d76bc38c8b9c182d1ac2`
-	Default Command: `["bash"]`

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
# Fri, 18 Jun 2021 02:03:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 02:04:05 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:09af03e0818b00fa01f51019b91f996a958b5ffb6b7dcd23e88d4d0df759f391`  
		Last Modified: Fri, 18 Jun 2021 02:07:59 GMT  
		Size: 129.1 MB (129059791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8` - linux; s390x

```console
$ docker pull ibmjava@sha256:e218d6e8e4a1fb597402e27fdba129d2dc4ed231b7f29d8c4fc9e62db9a2101e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154719490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2662465e7233122e8c18fdaca65d63466fe49a58df18cfd06e54cfdd161aa11`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:43:50 GMT
ADD file:cc2ee4aea9fbc14df65175678f3768999a62222c448822b8114b0adc46b28e9d in / 
# Thu, 17 Jun 2021 23:43:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:40:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:03 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:40:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:40:57 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:dc8b9e6580673058ca03527c82f177ec46b88568b02a42351a756002bdb90d3d`  
		Last Modified: Thu, 17 Jun 2021 23:45:21 GMT  
		Size: 25.4 MB (25366169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305ce5e190d86d73cebe54c653f38569a88806df13d166575044264699bd335`  
		Last Modified: Fri, 18 Jun 2021 00:43:16 GMT  
		Size: 2.7 MB (2676807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0166e67655d5cbb0bf2edbe0fae15d252659a53f14e27473e5650281b3b1f98`  
		Last Modified: Fri, 18 Jun 2021 00:43:24 GMT  
		Size: 126.7 MB (126676514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-jre`

```console
$ docker pull ibmjava@sha256:2c15590702d6a77ffa99a34f0c96a8bd7fd4f5a8248067564b7d5e15c26e719d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-jre` - linux; amd64

```console
$ docker pull ibmjava@sha256:57b1e6a944d9e2946516fc102d45d45e9d970a89b94963503f4c16324bafb2d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.2 MB (159196341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88d22d1bd2ef5ecabe40773943bc721e0c4500375984bb33d941198da6e836a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:26:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 01:26:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:26:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 01:27:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 01:27:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff3851d5fd9b952f0838f935196e2af17f7b597965441e75928bd4a7c7fda14`  
		Last Modified: Fri, 18 Jun 2021 01:29:04 GMT  
		Size: 3.0 MB (2959474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501e9b2fcdbe46c416058775ecae3071cb3a5182dfb4747ecb6775ea313b6b22`  
		Last Modified: Fri, 18 Jun 2021 01:29:13 GMT  
		Size: 129.5 MB (129536161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-jre` - linux; 386

```console
$ docker pull ibmjava@sha256:66e66e06954ce313b3d6295eff2a0a8825f4f4de3e09d77b454be4a0b1b5aa56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147864344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb4dd151fcd34a2577fdc78b167711bee47aa2d0e521ce92c47c1cd22b05cc3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:47:53 GMT
ADD file:3065820b37abf9a8ea82d39405ed55dc52d1e1ae7591a0a9d1c8a64e7287e06d in / 
# Thu, 17 Jun 2021 23:47:54 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:20:56 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:21:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:21:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:21:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:21:41 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:f76fac8c74a781007cb52b5223c59c8f3908bc41ecf0ae8f6dc9046b0aa24e58`  
		Last Modified: Thu, 17 Jun 2021 23:48:46 GMT  
		Size: 27.1 MB (27146196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5384f13a1fdaed1da8671f29859baba07658d2cb4ebdc38e420afb1856bb66`  
		Last Modified: Fri, 18 Jun 2021 00:23:42 GMT  
		Size: 3.0 MB (2987983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e0d59c7eca714b5a641beceded38d52ca85d0d9c6248bcfef384791113cc43`  
		Last Modified: Fri, 18 Jun 2021 00:23:54 GMT  
		Size: 117.7 MB (117730165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-jre` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:5b9acd7af8fd6f362c2d1e28666902aa815df5241ec8a0e43f36a8b5091fc561
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162568110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589254cf8583fa55985ef5cd52338ffb045060ffae67d76bc38c8b9c182d1ac2`
-	Default Command: `["bash"]`

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
# Fri, 18 Jun 2021 02:03:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 02:04:05 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:09af03e0818b00fa01f51019b91f996a958b5ffb6b7dcd23e88d4d0df759f391`  
		Last Modified: Fri, 18 Jun 2021 02:07:59 GMT  
		Size: 129.1 MB (129059791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-jre` - linux; s390x

```console
$ docker pull ibmjava@sha256:e218d6e8e4a1fb597402e27fdba129d2dc4ed231b7f29d8c4fc9e62db9a2101e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154719490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2662465e7233122e8c18fdaca65d63466fe49a58df18cfd06e54cfdd161aa11`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:43:50 GMT
ADD file:cc2ee4aea9fbc14df65175678f3768999a62222c448822b8114b0adc46b28e9d in / 
# Thu, 17 Jun 2021 23:43:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:40:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:03 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:40:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:40:57 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:dc8b9e6580673058ca03527c82f177ec46b88568b02a42351a756002bdb90d3d`  
		Last Modified: Thu, 17 Jun 2021 23:45:21 GMT  
		Size: 25.4 MB (25366169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305ce5e190d86d73cebe54c653f38569a88806df13d166575044264699bd335`  
		Last Modified: Fri, 18 Jun 2021 00:43:16 GMT  
		Size: 2.7 MB (2676807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0166e67655d5cbb0bf2edbe0fae15d252659a53f14e27473e5650281b3b1f98`  
		Last Modified: Fri, 18 Jun 2021 00:43:24 GMT  
		Size: 126.7 MB (126676514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-jre-alpine`

```console
$ docker pull ibmjava@sha256:f1752a725461929b425728e7413aef10e927ff3383e3a1cfe3139d1a95a291c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:8-jre-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:8e808a67bdda727109aba805b626e34816afdb466ff86dab6bf885c490d5eb4a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137893422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c67fe1857a7c18788046285d2790966a7667e36f7537613222a3bbd3bad514`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:52:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Apr 2021 22:52:22 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Wed, 14 Apr 2021 22:52:39 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Thu, 03 Jun 2021 21:24:53 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Thu, 03 Jun 2021 21:25:28 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Thu, 03 Jun 2021 21:25:28 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473651455a528e12a77a3f77634a9edcf271c6673a5d553738621ea93c7f661`  
		Last Modified: Wed, 14 Apr 2021 22:54:59 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a476c88f89042a64d394f56be791c17d185be12546f3f0be1966502a0643c`  
		Last Modified: Wed, 14 Apr 2021 22:55:01 GMT  
		Size: 5.5 MB (5539744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6854ed6de97957a8d470b8cbf8da87faffaf82b788ed64a016fd365e0e2a74f6`  
		Last Modified: Thu, 03 Jun 2021 21:28:54 GMT  
		Size: 129.6 MB (129552572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sdk`

```console
$ docker pull ibmjava@sha256:d5d82a084d41ea41f6a2738f22127c45d1762bdcc19a9704cf4bd48a34516a7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:8185ffde1a6085ef08da6cbbff6e834e1f16ead8ea7495365d99507a374bd00e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196341222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822bdc36ebdf66c64bd577ae9fc9f973681ff48ebfe6662634e7703d1bddc1fa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:26:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 01:26:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:26:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 01:28:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ebb0fd9e7e49b541663ea152a4c28b4d85c458fb00a35e407bfd922fea418fae';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dcf59f47f74e6ab9b9b1b36f17f31ce9ae800a54d3f8911ee4380a5f128071d7';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='124006e81d5fb148face2142ff7b6155c62876c6f819844d2d34d8d174a0efe7';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='46e8263da8b7cd80b780f5a9dbdab4f0000c32907af1ecbfe58edfc3068810e7';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='73fb5069d838eeeecbb801c4a8a03180a96e724dad79ef1b441be36ee8d53195';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 01:28:40 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff3851d5fd9b952f0838f935196e2af17f7b597965441e75928bd4a7c7fda14`  
		Last Modified: Fri, 18 Jun 2021 01:29:04 GMT  
		Size: 3.0 MB (2959474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fb3518f045ccbc5da4ec7b14f242260287f8fa6f79158f27d3de6e554602e0`  
		Last Modified: Fri, 18 Jun 2021 01:29:57 GMT  
		Size: 166.7 MB (166681042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:9d78acf7618476e83d3c969c309482284827414fb9290d2031ff7cc084131098
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.9 MB (184881108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23aee42d1dd714d9a3e870c563a1da3493560dbecf0fc0dda15e405d6bf8b7a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:47:53 GMT
ADD file:3065820b37abf9a8ea82d39405ed55dc52d1e1ae7591a0a9d1c8a64e7287e06d in / 
# Thu, 17 Jun 2021 23:47:54 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:20:56 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:21:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:21:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:23:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ebb0fd9e7e49b541663ea152a4c28b4d85c458fb00a35e407bfd922fea418fae';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dcf59f47f74e6ab9b9b1b36f17f31ce9ae800a54d3f8911ee4380a5f128071d7';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='124006e81d5fb148face2142ff7b6155c62876c6f819844d2d34d8d174a0efe7';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='46e8263da8b7cd80b780f5a9dbdab4f0000c32907af1ecbfe58edfc3068810e7';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='73fb5069d838eeeecbb801c4a8a03180a96e724dad79ef1b441be36ee8d53195';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:23:12 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:f76fac8c74a781007cb52b5223c59c8f3908bc41ecf0ae8f6dc9046b0aa24e58`  
		Last Modified: Thu, 17 Jun 2021 23:48:46 GMT  
		Size: 27.1 MB (27146196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5384f13a1fdaed1da8671f29859baba07658d2cb4ebdc38e420afb1856bb66`  
		Last Modified: Fri, 18 Jun 2021 00:23:42 GMT  
		Size: 3.0 MB (2987983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eb97a2bc13005087b31038a7072bf4f4755757944fd7558a4b5d6600a7e1bd`  
		Last Modified: Fri, 18 Jun 2021 00:24:46 GMT  
		Size: 154.7 MB (154746929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:20c208f1e6e975e405fd83ae10d5d5955cad60823eb9a99f5a99fe8e1759076c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.8 MB (199847013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7a723a7b476ff30f120c60ae14a92e3a2b620a0e5d9bbc356f6b69fb4e8fa88`
-	Default Command: `["bash"]`

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

### `ibmjava:8-sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:8e36d5c912959470216a02d30213194978d2eaa68d53d80c55d9004a1a3d1175
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.0 MB (185002477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e48208b4c0cd4b21f77472472a6b25b00f07bb5ba25c9fde1dc1c4b19e592d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:43:50 GMT
ADD file:cc2ee4aea9fbc14df65175678f3768999a62222c448822b8114b0adc46b28e9d in / 
# Thu, 17 Jun 2021 23:43:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:40:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:03 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:42:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ebb0fd9e7e49b541663ea152a4c28b4d85c458fb00a35e407bfd922fea418fae';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dcf59f47f74e6ab9b9b1b36f17f31ce9ae800a54d3f8911ee4380a5f128071d7';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='124006e81d5fb148face2142ff7b6155c62876c6f819844d2d34d8d174a0efe7';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='46e8263da8b7cd80b780f5a9dbdab4f0000c32907af1ecbfe58edfc3068810e7';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='73fb5069d838eeeecbb801c4a8a03180a96e724dad79ef1b441be36ee8d53195';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:43:01 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:dc8b9e6580673058ca03527c82f177ec46b88568b02a42351a756002bdb90d3d`  
		Last Modified: Thu, 17 Jun 2021 23:45:21 GMT  
		Size: 25.4 MB (25366169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305ce5e190d86d73cebe54c653f38569a88806df13d166575044264699bd335`  
		Last Modified: Fri, 18 Jun 2021 00:43:16 GMT  
		Size: 2.7 MB (2676807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424526fbe7e5071b6242a7fb9b2b0db3594fe4851ad1a29b0e7ac43aafaa45e`  
		Last Modified: Fri, 18 Jun 2021 00:43:57 GMT  
		Size: 157.0 MB (156959501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sdk-alpine`

```console
$ docker pull ibmjava@sha256:1fe4106ffc54495c215ee6a3c8bac11a7ad34e82b2f9950d834e0705d2e37c99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:8-sdk-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:7bb1ec5f0be168dec4797885c0dfb53d98886dfd01879bfed592a44349d0ef63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.0 MB (175033632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faeda7a451479203ef04c1f4077208a2607832862a6a722ac5bfc7bf36c04b9b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:52:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Apr 2021 22:52:22 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Wed, 14 Apr 2021 22:52:39 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Thu, 03 Jun 2021 21:24:53 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Thu, 03 Jun 2021 21:27:55 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ebb0fd9e7e49b541663ea152a4c28b4d85c458fb00a35e407bfd922fea418fae';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dcf59f47f74e6ab9b9b1b36f17f31ce9ae800a54d3f8911ee4380a5f128071d7';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='124006e81d5fb148face2142ff7b6155c62876c6f819844d2d34d8d174a0efe7';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='46e8263da8b7cd80b780f5a9dbdab4f0000c32907af1ecbfe58edfc3068810e7';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='73fb5069d838eeeecbb801c4a8a03180a96e724dad79ef1b441be36ee8d53195';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Thu, 03 Jun 2021 21:27:56 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473651455a528e12a77a3f77634a9edcf271c6673a5d553738621ea93c7f661`  
		Last Modified: Wed, 14 Apr 2021 22:54:59 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a476c88f89042a64d394f56be791c17d185be12546f3f0be1966502a0643c`  
		Last Modified: Wed, 14 Apr 2021 22:55:01 GMT  
		Size: 5.5 MB (5539744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8169a114fdc61189630b383edeffe0f6190a90494d0f4f86f22da251624963`  
		Last Modified: Thu, 03 Jun 2021 21:30:11 GMT  
		Size: 166.7 MB (166692782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sfj`

```console
$ docker pull ibmjava@sha256:b437b9e25e6b9dd16302183ac21ee2355f3104d014399d735e9c5ff5ba285740
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:cba04437e8b757edde036f0d209d3cb9045ec4542128265bdee958b8b6d53030
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94030718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0ea5927597fc5e2f63e4751795ba0ea509786c0f302c45b0a5791e73ba9b7d2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:26:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 01:26:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:26:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 01:27:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 01:27:54 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff3851d5fd9b952f0838f935196e2af17f7b597965441e75928bd4a7c7fda14`  
		Last Modified: Fri, 18 Jun 2021 01:29:04 GMT  
		Size: 3.0 MB (2959474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5f8d75d97fd32798feab6e3bd63f6f820b9611d4a019369b091a22d4e3ef76`  
		Last Modified: Fri, 18 Jun 2021 01:29:34 GMT  
		Size: 64.4 MB (64370538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:6eab4647864f2f9606365f701fb0f7c8ead2028881e55dc22f58f3cabc2b77b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93871302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad362c6e4bcc09a3d0d357d043852ef12798120d908bd7b0920bd47d32c10dbd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:47:53 GMT
ADD file:3065820b37abf9a8ea82d39405ed55dc52d1e1ae7591a0a9d1c8a64e7287e06d in / 
# Thu, 17 Jun 2021 23:47:54 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:20:56 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:21:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:21:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:22:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:22:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:f76fac8c74a781007cb52b5223c59c8f3908bc41ecf0ae8f6dc9046b0aa24e58`  
		Last Modified: Thu, 17 Jun 2021 23:48:46 GMT  
		Size: 27.1 MB (27146196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5384f13a1fdaed1da8671f29859baba07658d2cb4ebdc38e420afb1856bb66`  
		Last Modified: Fri, 18 Jun 2021 00:23:42 GMT  
		Size: 3.0 MB (2987983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823592fa3a3cfc360e9341f9af35d926e8901df2824a8496c401b83e64123752`  
		Last Modified: Fri, 18 Jun 2021 00:24:20 GMT  
		Size: 63.7 MB (63737123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:b58dce5a36790039ec35f8845ed7a680025ea4329a62fd78d4eff35730a21710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103226494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348d7e9171b88637deaf917ac8e3d4b4ea71b87d54d8257d23cdeebcd7fe74c8`
-	Default Command: `["bash"]`

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
# Fri, 18 Jun 2021 02:05:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 02:05:20 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:f2a0432a089b642e2441a048b31f2f92a025d959ae059bdcf61481e13605d997`  
		Last Modified: Fri, 18 Jun 2021 02:08:22 GMT  
		Size: 69.7 MB (69718175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:5f733298fcafa554c15b4185ce20bb1575c009f80bbb9a3078c06595e178c280
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.5 MB (93511174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2111888b043203242247b0068657721bb14143c3e23d730cc279f6c3d4b17195`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:43:50 GMT
ADD file:cc2ee4aea9fbc14df65175678f3768999a62222c448822b8114b0adc46b28e9d in / 
# Thu, 17 Jun 2021 23:43:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:40:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:03 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:41:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:41:47 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:dc8b9e6580673058ca03527c82f177ec46b88568b02a42351a756002bdb90d3d`  
		Last Modified: Thu, 17 Jun 2021 23:45:21 GMT  
		Size: 25.4 MB (25366169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305ce5e190d86d73cebe54c653f38569a88806df13d166575044264699bd335`  
		Last Modified: Fri, 18 Jun 2021 00:43:16 GMT  
		Size: 2.7 MB (2676807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f274719f86efc060ef2affcbfecf82e2bf540ac43bef6aa638a1fa9a7887ed`  
		Last Modified: Fri, 18 Jun 2021 00:43:40 GMT  
		Size: 65.5 MB (65468198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sfj-alpine`

```console
$ docker pull ibmjava@sha256:262e9812cc0f11c41e15218cc64a4ab9a9cadb899c8112659b2730dd435112be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:8-sfj-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:f20484e24cee6fefbd379345f6296e334948933bdacbd1cc577157cd055fa053
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72730682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f698c6b09cd03fb877f7156778ebe0de810f7ec8eb5d5e741371befa41e6e6cb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:52:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Apr 2021 22:52:22 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Wed, 14 Apr 2021 22:52:39 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Thu, 03 Jun 2021 21:24:53 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Thu, 03 Jun 2021 21:26:31 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Thu, 03 Jun 2021 21:26:31 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473651455a528e12a77a3f77634a9edcf271c6673a5d553738621ea93c7f661`  
		Last Modified: Wed, 14 Apr 2021 22:54:59 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a476c88f89042a64d394f56be791c17d185be12546f3f0be1966502a0643c`  
		Last Modified: Wed, 14 Apr 2021 22:55:01 GMT  
		Size: 5.5 MB (5539744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82faec9364eaa46bdef7684300da3856f837389a970f23de2f4391af423bbd2`  
		Last Modified: Thu, 03 Jun 2021 21:29:27 GMT  
		Size: 64.4 MB (64389832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:jre`

```console
$ docker pull ibmjava@sha256:2c15590702d6a77ffa99a34f0c96a8bd7fd4f5a8248067564b7d5e15c26e719d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:jre` - linux; amd64

```console
$ docker pull ibmjava@sha256:57b1e6a944d9e2946516fc102d45d45e9d970a89b94963503f4c16324bafb2d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.2 MB (159196341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88d22d1bd2ef5ecabe40773943bc721e0c4500375984bb33d941198da6e836a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:26:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 01:26:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:26:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 01:27:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 01:27:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff3851d5fd9b952f0838f935196e2af17f7b597965441e75928bd4a7c7fda14`  
		Last Modified: Fri, 18 Jun 2021 01:29:04 GMT  
		Size: 3.0 MB (2959474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501e9b2fcdbe46c416058775ecae3071cb3a5182dfb4747ecb6775ea313b6b22`  
		Last Modified: Fri, 18 Jun 2021 01:29:13 GMT  
		Size: 129.5 MB (129536161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; 386

```console
$ docker pull ibmjava@sha256:66e66e06954ce313b3d6295eff2a0a8825f4f4de3e09d77b454be4a0b1b5aa56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147864344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb4dd151fcd34a2577fdc78b167711bee47aa2d0e521ce92c47c1cd22b05cc3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:47:53 GMT
ADD file:3065820b37abf9a8ea82d39405ed55dc52d1e1ae7591a0a9d1c8a64e7287e06d in / 
# Thu, 17 Jun 2021 23:47:54 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:20:56 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:21:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:21:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:21:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:21:41 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:f76fac8c74a781007cb52b5223c59c8f3908bc41ecf0ae8f6dc9046b0aa24e58`  
		Last Modified: Thu, 17 Jun 2021 23:48:46 GMT  
		Size: 27.1 MB (27146196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5384f13a1fdaed1da8671f29859baba07658d2cb4ebdc38e420afb1856bb66`  
		Last Modified: Fri, 18 Jun 2021 00:23:42 GMT  
		Size: 3.0 MB (2987983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e0d59c7eca714b5a641beceded38d52ca85d0d9c6248bcfef384791113cc43`  
		Last Modified: Fri, 18 Jun 2021 00:23:54 GMT  
		Size: 117.7 MB (117730165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:5b9acd7af8fd6f362c2d1e28666902aa815df5241ec8a0e43f36a8b5091fc561
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162568110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589254cf8583fa55985ef5cd52338ffb045060ffae67d76bc38c8b9c182d1ac2`
-	Default Command: `["bash"]`

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
# Fri, 18 Jun 2021 02:03:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 02:04:05 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:09af03e0818b00fa01f51019b91f996a958b5ffb6b7dcd23e88d4d0df759f391`  
		Last Modified: Fri, 18 Jun 2021 02:07:59 GMT  
		Size: 129.1 MB (129059791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; s390x

```console
$ docker pull ibmjava@sha256:e218d6e8e4a1fb597402e27fdba129d2dc4ed231b7f29d8c4fc9e62db9a2101e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154719490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2662465e7233122e8c18fdaca65d63466fe49a58df18cfd06e54cfdd161aa11`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:43:50 GMT
ADD file:cc2ee4aea9fbc14df65175678f3768999a62222c448822b8114b0adc46b28e9d in / 
# Thu, 17 Jun 2021 23:43:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:40:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:03 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:40:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:40:57 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:dc8b9e6580673058ca03527c82f177ec46b88568b02a42351a756002bdb90d3d`  
		Last Modified: Thu, 17 Jun 2021 23:45:21 GMT  
		Size: 25.4 MB (25366169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305ce5e190d86d73cebe54c653f38569a88806df13d166575044264699bd335`  
		Last Modified: Fri, 18 Jun 2021 00:43:16 GMT  
		Size: 2.7 MB (2676807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0166e67655d5cbb0bf2edbe0fae15d252659a53f14e27473e5650281b3b1f98`  
		Last Modified: Fri, 18 Jun 2021 00:43:24 GMT  
		Size: 126.7 MB (126676514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:jre-alpine`

```console
$ docker pull ibmjava@sha256:f1752a725461929b425728e7413aef10e927ff3383e3a1cfe3139d1a95a291c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:jre-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:8e808a67bdda727109aba805b626e34816afdb466ff86dab6bf885c490d5eb4a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137893422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c67fe1857a7c18788046285d2790966a7667e36f7537613222a3bbd3bad514`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:52:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Apr 2021 22:52:22 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Wed, 14 Apr 2021 22:52:39 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Thu, 03 Jun 2021 21:24:53 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Thu, 03 Jun 2021 21:25:28 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Thu, 03 Jun 2021 21:25:28 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473651455a528e12a77a3f77634a9edcf271c6673a5d553738621ea93c7f661`  
		Last Modified: Wed, 14 Apr 2021 22:54:59 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a476c88f89042a64d394f56be791c17d185be12546f3f0be1966502a0643c`  
		Last Modified: Wed, 14 Apr 2021 22:55:01 GMT  
		Size: 5.5 MB (5539744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6854ed6de97957a8d470b8cbf8da87faffaf82b788ed64a016fd365e0e2a74f6`  
		Last Modified: Thu, 03 Jun 2021 21:28:54 GMT  
		Size: 129.6 MB (129552572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:latest`

```console
$ docker pull ibmjava@sha256:2c15590702d6a77ffa99a34f0c96a8bd7fd4f5a8248067564b7d5e15c26e719d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:latest` - linux; amd64

```console
$ docker pull ibmjava@sha256:57b1e6a944d9e2946516fc102d45d45e9d970a89b94963503f4c16324bafb2d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.2 MB (159196341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88d22d1bd2ef5ecabe40773943bc721e0c4500375984bb33d941198da6e836a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:26:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 01:26:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:26:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 01:27:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 01:27:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff3851d5fd9b952f0838f935196e2af17f7b597965441e75928bd4a7c7fda14`  
		Last Modified: Fri, 18 Jun 2021 01:29:04 GMT  
		Size: 3.0 MB (2959474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501e9b2fcdbe46c416058775ecae3071cb3a5182dfb4747ecb6775ea313b6b22`  
		Last Modified: Fri, 18 Jun 2021 01:29:13 GMT  
		Size: 129.5 MB (129536161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; 386

```console
$ docker pull ibmjava@sha256:66e66e06954ce313b3d6295eff2a0a8825f4f4de3e09d77b454be4a0b1b5aa56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147864344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb4dd151fcd34a2577fdc78b167711bee47aa2d0e521ce92c47c1cd22b05cc3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:47:53 GMT
ADD file:3065820b37abf9a8ea82d39405ed55dc52d1e1ae7591a0a9d1c8a64e7287e06d in / 
# Thu, 17 Jun 2021 23:47:54 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:20:56 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:21:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:21:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:21:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:21:41 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:f76fac8c74a781007cb52b5223c59c8f3908bc41ecf0ae8f6dc9046b0aa24e58`  
		Last Modified: Thu, 17 Jun 2021 23:48:46 GMT  
		Size: 27.1 MB (27146196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5384f13a1fdaed1da8671f29859baba07658d2cb4ebdc38e420afb1856bb66`  
		Last Modified: Fri, 18 Jun 2021 00:23:42 GMT  
		Size: 3.0 MB (2987983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e0d59c7eca714b5a641beceded38d52ca85d0d9c6248bcfef384791113cc43`  
		Last Modified: Fri, 18 Jun 2021 00:23:54 GMT  
		Size: 117.7 MB (117730165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:5b9acd7af8fd6f362c2d1e28666902aa815df5241ec8a0e43f36a8b5091fc561
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162568110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589254cf8583fa55985ef5cd52338ffb045060ffae67d76bc38c8b9c182d1ac2`
-	Default Command: `["bash"]`

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
# Fri, 18 Jun 2021 02:03:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 02:04:05 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:09af03e0818b00fa01f51019b91f996a958b5ffb6b7dcd23e88d4d0df759f391`  
		Last Modified: Fri, 18 Jun 2021 02:07:59 GMT  
		Size: 129.1 MB (129059791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; s390x

```console
$ docker pull ibmjava@sha256:e218d6e8e4a1fb597402e27fdba129d2dc4ed231b7f29d8c4fc9e62db9a2101e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154719490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2662465e7233122e8c18fdaca65d63466fe49a58df18cfd06e54cfdd161aa11`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:43:50 GMT
ADD file:cc2ee4aea9fbc14df65175678f3768999a62222c448822b8114b0adc46b28e9d in / 
# Thu, 17 Jun 2021 23:43:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:40:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:03 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:40:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ed09900a0219b40ddfa06098118a701b8633dcf12588e13ff8b7d810ef2769dc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='95bf8be233306b046150b949d2a8b9ce604eb6f4a090aaa7bf54152181fcdc06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='b6a57eff545b75f6fe164c0e96eab56d1a889ae7574e205230f84175b50f6c03';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2b2b73eef781996e570670a2dec541778647a2afb37b516c9a750e7857fc90aa';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='70da4d42a8181e7a13ca63320acf856315b993f35222e34fa50032a270d472d4';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:40:57 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:dc8b9e6580673058ca03527c82f177ec46b88568b02a42351a756002bdb90d3d`  
		Last Modified: Thu, 17 Jun 2021 23:45:21 GMT  
		Size: 25.4 MB (25366169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305ce5e190d86d73cebe54c653f38569a88806df13d166575044264699bd335`  
		Last Modified: Fri, 18 Jun 2021 00:43:16 GMT  
		Size: 2.7 MB (2676807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0166e67655d5cbb0bf2edbe0fae15d252659a53f14e27473e5650281b3b1f98`  
		Last Modified: Fri, 18 Jun 2021 00:43:24 GMT  
		Size: 126.7 MB (126676514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sdk`

```console
$ docker pull ibmjava@sha256:d5d82a084d41ea41f6a2738f22127c45d1762bdcc19a9704cf4bd48a34516a7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:8185ffde1a6085ef08da6cbbff6e834e1f16ead8ea7495365d99507a374bd00e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196341222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822bdc36ebdf66c64bd577ae9fc9f973681ff48ebfe6662634e7703d1bddc1fa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:26:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 01:26:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:26:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 01:28:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ebb0fd9e7e49b541663ea152a4c28b4d85c458fb00a35e407bfd922fea418fae';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dcf59f47f74e6ab9b9b1b36f17f31ce9ae800a54d3f8911ee4380a5f128071d7';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='124006e81d5fb148face2142ff7b6155c62876c6f819844d2d34d8d174a0efe7';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='46e8263da8b7cd80b780f5a9dbdab4f0000c32907af1ecbfe58edfc3068810e7';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='73fb5069d838eeeecbb801c4a8a03180a96e724dad79ef1b441be36ee8d53195';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 01:28:40 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff3851d5fd9b952f0838f935196e2af17f7b597965441e75928bd4a7c7fda14`  
		Last Modified: Fri, 18 Jun 2021 01:29:04 GMT  
		Size: 3.0 MB (2959474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fb3518f045ccbc5da4ec7b14f242260287f8fa6f79158f27d3de6e554602e0`  
		Last Modified: Fri, 18 Jun 2021 01:29:57 GMT  
		Size: 166.7 MB (166681042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:9d78acf7618476e83d3c969c309482284827414fb9290d2031ff7cc084131098
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.9 MB (184881108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23aee42d1dd714d9a3e870c563a1da3493560dbecf0fc0dda15e405d6bf8b7a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:47:53 GMT
ADD file:3065820b37abf9a8ea82d39405ed55dc52d1e1ae7591a0a9d1c8a64e7287e06d in / 
# Thu, 17 Jun 2021 23:47:54 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:20:56 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:21:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:21:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:23:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ebb0fd9e7e49b541663ea152a4c28b4d85c458fb00a35e407bfd922fea418fae';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dcf59f47f74e6ab9b9b1b36f17f31ce9ae800a54d3f8911ee4380a5f128071d7';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='124006e81d5fb148face2142ff7b6155c62876c6f819844d2d34d8d174a0efe7';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='46e8263da8b7cd80b780f5a9dbdab4f0000c32907af1ecbfe58edfc3068810e7';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='73fb5069d838eeeecbb801c4a8a03180a96e724dad79ef1b441be36ee8d53195';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:23:12 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:f76fac8c74a781007cb52b5223c59c8f3908bc41ecf0ae8f6dc9046b0aa24e58`  
		Last Modified: Thu, 17 Jun 2021 23:48:46 GMT  
		Size: 27.1 MB (27146196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5384f13a1fdaed1da8671f29859baba07658d2cb4ebdc38e420afb1856bb66`  
		Last Modified: Fri, 18 Jun 2021 00:23:42 GMT  
		Size: 3.0 MB (2987983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eb97a2bc13005087b31038a7072bf4f4755757944fd7558a4b5d6600a7e1bd`  
		Last Modified: Fri, 18 Jun 2021 00:24:46 GMT  
		Size: 154.7 MB (154746929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:20c208f1e6e975e405fd83ae10d5d5955cad60823eb9a99f5a99fe8e1759076c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.8 MB (199847013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7a723a7b476ff30f120c60ae14a92e3a2b620a0e5d9bbc356f6b69fb4e8fa88`
-	Default Command: `["bash"]`

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

### `ibmjava:sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:8e36d5c912959470216a02d30213194978d2eaa68d53d80c55d9004a1a3d1175
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.0 MB (185002477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e48208b4c0cd4b21f77472472a6b25b00f07bb5ba25c9fde1dc1c4b19e592d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:43:50 GMT
ADD file:cc2ee4aea9fbc14df65175678f3768999a62222c448822b8114b0adc46b28e9d in / 
# Thu, 17 Jun 2021 23:43:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:40:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:03 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:42:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ebb0fd9e7e49b541663ea152a4c28b4d85c458fb00a35e407bfd922fea418fae';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dcf59f47f74e6ab9b9b1b36f17f31ce9ae800a54d3f8911ee4380a5f128071d7';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='124006e81d5fb148face2142ff7b6155c62876c6f819844d2d34d8d174a0efe7';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='46e8263da8b7cd80b780f5a9dbdab4f0000c32907af1ecbfe58edfc3068810e7';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='73fb5069d838eeeecbb801c4a8a03180a96e724dad79ef1b441be36ee8d53195';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:43:01 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:dc8b9e6580673058ca03527c82f177ec46b88568b02a42351a756002bdb90d3d`  
		Last Modified: Thu, 17 Jun 2021 23:45:21 GMT  
		Size: 25.4 MB (25366169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305ce5e190d86d73cebe54c653f38569a88806df13d166575044264699bd335`  
		Last Modified: Fri, 18 Jun 2021 00:43:16 GMT  
		Size: 2.7 MB (2676807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424526fbe7e5071b6242a7fb9b2b0db3594fe4851ad1a29b0e7ac43aafaa45e`  
		Last Modified: Fri, 18 Jun 2021 00:43:57 GMT  
		Size: 157.0 MB (156959501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sdk-alpine`

```console
$ docker pull ibmjava@sha256:1fe4106ffc54495c215ee6a3c8bac11a7ad34e82b2f9950d834e0705d2e37c99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:sdk-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:7bb1ec5f0be168dec4797885c0dfb53d98886dfd01879bfed592a44349d0ef63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.0 MB (175033632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faeda7a451479203ef04c1f4077208a2607832862a6a722ac5bfc7bf36c04b9b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:52:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Apr 2021 22:52:22 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Wed, 14 Apr 2021 22:52:39 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Thu, 03 Jun 2021 21:24:53 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Thu, 03 Jun 2021 21:27:55 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ebb0fd9e7e49b541663ea152a4c28b4d85c458fb00a35e407bfd922fea418fae';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dcf59f47f74e6ab9b9b1b36f17f31ce9ae800a54d3f8911ee4380a5f128071d7';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='124006e81d5fb148face2142ff7b6155c62876c6f819844d2d34d8d174a0efe7';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='46e8263da8b7cd80b780f5a9dbdab4f0000c32907af1ecbfe58edfc3068810e7';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='73fb5069d838eeeecbb801c4a8a03180a96e724dad79ef1b441be36ee8d53195';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Thu, 03 Jun 2021 21:27:56 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473651455a528e12a77a3f77634a9edcf271c6673a5d553738621ea93c7f661`  
		Last Modified: Wed, 14 Apr 2021 22:54:59 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a476c88f89042a64d394f56be791c17d185be12546f3f0be1966502a0643c`  
		Last Modified: Wed, 14 Apr 2021 22:55:01 GMT  
		Size: 5.5 MB (5539744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8169a114fdc61189630b383edeffe0f6190a90494d0f4f86f22da251624963`  
		Last Modified: Thu, 03 Jun 2021 21:30:11 GMT  
		Size: 166.7 MB (166692782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sfj`

```console
$ docker pull ibmjava@sha256:b437b9e25e6b9dd16302183ac21ee2355f3104d014399d735e9c5ff5ba285740
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:cba04437e8b757edde036f0d209d3cb9045ec4542128265bdee958b8b6d53030
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94030718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0ea5927597fc5e2f63e4751795ba0ea509786c0f302c45b0a5791e73ba9b7d2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:26:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 01:26:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:26:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 01:27:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 01:27:54 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff3851d5fd9b952f0838f935196e2af17f7b597965441e75928bd4a7c7fda14`  
		Last Modified: Fri, 18 Jun 2021 01:29:04 GMT  
		Size: 3.0 MB (2959474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5f8d75d97fd32798feab6e3bd63f6f820b9611d4a019369b091a22d4e3ef76`  
		Last Modified: Fri, 18 Jun 2021 01:29:34 GMT  
		Size: 64.4 MB (64370538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:6eab4647864f2f9606365f701fb0f7c8ead2028881e55dc22f58f3cabc2b77b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93871302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad362c6e4bcc09a3d0d357d043852ef12798120d908bd7b0920bd47d32c10dbd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:47:53 GMT
ADD file:3065820b37abf9a8ea82d39405ed55dc52d1e1ae7591a0a9d1c8a64e7287e06d in / 
# Thu, 17 Jun 2021 23:47:54 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:20:56 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:21:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:21:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:22:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:22:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:f76fac8c74a781007cb52b5223c59c8f3908bc41ecf0ae8f6dc9046b0aa24e58`  
		Last Modified: Thu, 17 Jun 2021 23:48:46 GMT  
		Size: 27.1 MB (27146196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5384f13a1fdaed1da8671f29859baba07658d2cb4ebdc38e420afb1856bb66`  
		Last Modified: Fri, 18 Jun 2021 00:23:42 GMT  
		Size: 3.0 MB (2987983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823592fa3a3cfc360e9341f9af35d926e8901df2824a8496c401b83e64123752`  
		Last Modified: Fri, 18 Jun 2021 00:24:20 GMT  
		Size: 63.7 MB (63737123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:b58dce5a36790039ec35f8845ed7a680025ea4329a62fd78d4eff35730a21710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103226494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348d7e9171b88637deaf917ac8e3d4b4ea71b87d54d8257d23cdeebcd7fe74c8`
-	Default Command: `["bash"]`

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
# Fri, 18 Jun 2021 02:05:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 02:05:20 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:f2a0432a089b642e2441a048b31f2f92a025d959ae059bdcf61481e13605d997`  
		Last Modified: Fri, 18 Jun 2021 02:08:22 GMT  
		Size: 69.7 MB (69718175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:5f733298fcafa554c15b4185ce20bb1575c009f80bbb9a3078c06595e178c280
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.5 MB (93511174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2111888b043203242247b0068657721bb14143c3e23d730cc279f6c3d4b17195`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:43:50 GMT
ADD file:cc2ee4aea9fbc14df65175678f3768999a62222c448822b8114b0adc46b28e9d in / 
# Thu, 17 Jun 2021 23:43:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:39:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 18 Jun 2021 00:40:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:03 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Fri, 18 Jun 2021 00:41:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 18 Jun 2021 00:41:47 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:dc8b9e6580673058ca03527c82f177ec46b88568b02a42351a756002bdb90d3d`  
		Last Modified: Thu, 17 Jun 2021 23:45:21 GMT  
		Size: 25.4 MB (25366169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305ce5e190d86d73cebe54c653f38569a88806df13d166575044264699bd335`  
		Last Modified: Fri, 18 Jun 2021 00:43:16 GMT  
		Size: 2.7 MB (2676807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f274719f86efc060ef2affcbfecf82e2bf540ac43bef6aa638a1fa9a7887ed`  
		Last Modified: Fri, 18 Jun 2021 00:43:40 GMT  
		Size: 65.5 MB (65468198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sfj-alpine`

```console
$ docker pull ibmjava@sha256:262e9812cc0f11c41e15218cc64a4ab9a9cadb899c8112659b2730dd435112be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:sfj-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:f20484e24cee6fefbd379345f6296e334948933bdacbd1cc577157cd055fa053
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72730682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f698c6b09cd03fb877f7156778ebe0de810f7ec8eb5d5e741371befa41e6e6cb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:52:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Apr 2021 22:52:22 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Wed, 14 Apr 2021 22:52:39 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Thu, 03 Jun 2021 21:24:53 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Thu, 03 Jun 2021 21:26:31 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Thu, 03 Jun 2021 21:26:31 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473651455a528e12a77a3f77634a9edcf271c6673a5d553738621ea93c7f661`  
		Last Modified: Wed, 14 Apr 2021 22:54:59 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a476c88f89042a64d394f56be791c17d185be12546f3f0be1966502a0643c`  
		Last Modified: Wed, 14 Apr 2021 22:55:01 GMT  
		Size: 5.5 MB (5539744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82faec9364eaa46bdef7684300da3856f837389a970f23de2f4391af423bbd2`  
		Last Modified: Thu, 03 Jun 2021 21:29:27 GMT  
		Size: 64.4 MB (64389832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
