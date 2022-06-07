## `ibmjava:sdk`

```console
$ docker pull ibmjava@sha256:16367f5845fbec2d366533d3cacf67f1115d7ee7c982ec71393c774c5cb6510a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:3d30d91f7912cb6a96081184c3d89393e17cbda0fe5165ee803abf6e4ce11555
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.9 MB (195875461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:116710b66ed307d222d38dd01c2d2e1e5048b3d14999d47428f1550e359a32a9`
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
# Tue, 07 Jun 2022 02:52:40 GMT
ENV JAVA_VERSION=8.0.7.10
# Tue, 07 Jun 2022 02:54:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='29261a59ea6675033eb5b7a741dbb52692777f4823ec72f7111519be6eaa7f98';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='4cacce0b93b178d1ef45e15e0d80cc1b138f57955dd0735d8eaee833e1cc61e7';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='2b422324023b547e25b25a6ab83cafafc63f90e82c42dbb70dc285009e65f5e3';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='62f7d58c80d5d0b014a26ff1442711f1d0bc52ec671640e6f1fb00ca867edf2c';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='03238fd859bf16f958492cf9af172b70a94a5ec0df405eda2d1f0d69cfcc520c';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 07 Jun 2022 02:54:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:a33a97ebca46987bd412558b5d84deb010c0e6b342947fe3455369cd288fc516`  
		Last Modified: Tue, 07 Jun 2022 02:55:46 GMT  
		Size: 166.2 MB (166203615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:1c1bb4e50a7ca8235a16591fee75cd3b1dcf8d57e12bea3b75537fe673053b21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.5 MB (184490269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce02137be81b1c9ef7d84cb37fdebbbaac763fd8bad20e98444b2785ec83de4`
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
# Mon, 06 Jun 2022 21:52:37 GMT
ENV JAVA_VERSION=8.0.7.10
# Mon, 06 Jun 2022 21:54:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='29261a59ea6675033eb5b7a741dbb52692777f4823ec72f7111519be6eaa7f98';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='4cacce0b93b178d1ef45e15e0d80cc1b138f57955dd0735d8eaee833e1cc61e7';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='2b422324023b547e25b25a6ab83cafafc63f90e82c42dbb70dc285009e65f5e3';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='62f7d58c80d5d0b014a26ff1442711f1d0bc52ec671640e6f1fb00ca867edf2c';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='03238fd859bf16f958492cf9af172b70a94a5ec0df405eda2d1f0d69cfcc520c';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Mon, 06 Jun 2022 21:54:40 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:60f01a061eb37904d80023965ae3eca72f1f3984ca7ec8fad4332297d4af68d9`  
		Last Modified: Mon, 06 Jun 2022 21:56:24 GMT  
		Size: 154.3 MB (154335808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:c44f18153c97a891809a95dcd5e924b7d739eba18eb9cb274afb4ddf1c6a5fba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.4 MB (199382167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:279c7e4c8774c130bb8c54e10e38e173314cc205c0be9bea86ebff6ebe59d469`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:00 GMT
ADD file:2d91cfcbab5facf9c027064efd477cfde81eca0c1a62c6611ac694bafb94d817 in / 
# Fri, 29 Apr 2022 23:22:04 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:49:39 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 30 Apr 2022 01:50:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Jun 2022 18:17:09 GMT
ENV JAVA_VERSION=8.0.7.10
# Wed, 01 Jun 2022 18:20:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='29261a59ea6675033eb5b7a741dbb52692777f4823ec72f7111519be6eaa7f98';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='4cacce0b93b178d1ef45e15e0d80cc1b138f57955dd0735d8eaee833e1cc61e7';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='2b422324023b547e25b25a6ab83cafafc63f90e82c42dbb70dc285009e65f5e3';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='62f7d58c80d5d0b014a26ff1442711f1d0bc52ec671640e6f1fb00ca867edf2c';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='03238fd859bf16f958492cf9af172b70a94a5ec0df405eda2d1f0d69cfcc520c';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 01 Jun 2022 18:20:41 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:c70b79613e1f9e69f0d6473fa0b3f8b10d376e24350617c381ed64978f4bae97`  
		Last Modified: Fri, 29 Apr 2022 23:24:58 GMT  
		Size: 30.4 MB (30443183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b9fc7dc4c2bad9d9f7db0ffd5b499212f90be1d458552dba4bd7e526ede046`  
		Last Modified: Sat, 30 Apr 2022 01:54:24 GMT  
		Size: 3.1 MB (3082255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e9210303c7b3fa6d54746d8b17d8d3644abc3d132b2cd93ed43f5453d02c45`  
		Last Modified: Wed, 01 Jun 2022 18:22:27 GMT  
		Size: 165.9 MB (165856729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:276def5403f1cde5f37313e0d93b17b3462ea8d3e3a855c48f69a9bcf8e19d9a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.4 MB (184413854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a24387fa1443f387af997d2435371c35c38c3f6a817d03891819fd9d9466ffe2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:50 GMT
ADD file:9b5ddd45fc485b5c5ea3d28339d1768fa5d8f60059022a971897d51d94ad5847 in / 
# Fri, 29 Apr 2022 22:49:54 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:27:15 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 29 Apr 2022 23:27:21 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Jun 2022 15:41:55 GMT
ENV JAVA_VERSION=8.0.7.10
# Wed, 01 Jun 2022 15:45:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='29261a59ea6675033eb5b7a741dbb52692777f4823ec72f7111519be6eaa7f98';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='4cacce0b93b178d1ef45e15e0d80cc1b138f57955dd0735d8eaee833e1cc61e7';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='2b422324023b547e25b25a6ab83cafafc63f90e82c42dbb70dc285009e65f5e3';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='62f7d58c80d5d0b014a26ff1442711f1d0bc52ec671640e6f1fb00ca867edf2c';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='03238fd859bf16f958492cf9af172b70a94a5ec0df405eda2d1f0d69cfcc520c';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 01 Jun 2022 15:45:33 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:1347a7b069ceb0e131b6f229b7b96bae189f8e4c594c1933170e278d0ed928b2`  
		Last Modified: Fri, 29 Apr 2022 22:51:49 GMT  
		Size: 25.4 MB (25365828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f94c1c13b8b89cf54909fe9580987f60938a39e09f8c39697300c3a17a3ec1`  
		Last Modified: Fri, 29 Apr 2022 23:30:09 GMT  
		Size: 2.7 MB (2677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74714c47ca980ce289290dcb186a69e0a7f40ac7d54a26c74236288414cd22d`  
		Last Modified: Wed, 01 Jun 2022 15:46:59 GMT  
		Size: 156.4 MB (156371010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
