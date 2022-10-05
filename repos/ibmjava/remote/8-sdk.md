## `ibmjava:8-sdk`

```console
$ docker pull ibmjava@sha256:7088463374a9b93252b61af632cf75d5962be28af42c5a7417ad21e6a43046f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:7bc24af5f114974b6bbf77d0588878d451765ef939c2ea11e2f8dbbac85969ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196167437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f301e8e7fef58bfa7395236a39455d69c8e608921c47107dbb6ff9985e4a32`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 17:13:23 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 05 Oct 2022 17:13:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:13:31 GMT
ENV JAVA_VERSION=8.0.7.16
# Wed, 05 Oct 2022 17:16:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bb34f647a77ae43611dab3a447da447686352da5426baaff26c22a465dfe40c0';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='b8c35301b56fde151b14e1bfb1374f579f5a0ed361d6ebc7ffff5f82eb563344';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='79fde4473b2c489278fdef105bf69097f1f1a0d54d75a59d24008773b512339b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f1989ee7f41d8d697e880dea74f94133841c2f59ded5c9dd551a26b87f4d36cf';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='eb1cd5b6bf532f10558e7067768d14884d9fce375d2782f91b2218365152bc42';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 05 Oct 2022 17:16:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9d8b98df188102d0298ec847e22cee30b83e6a2203144208de17a84f4e915a`  
		Last Modified: Wed, 05 Oct 2022 17:16:34 GMT  
		Size: 3.0 MB (2957821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a1a9a79dbef2c33332c84d69ba5ed351486e561c7a18a08dbb72dcc4f1bd50`  
		Last Modified: Wed, 05 Oct 2022 17:17:24 GMT  
		Size: 166.5 MB (166497764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:23b8b6df68b174a28a24308a041eb8595b932597a991aaca0a8392827784ff12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.7 MB (184652417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2446fdf64236272e7e7e90253844bdfbc50c1aeb5b01b06613c74ab1b4039079`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:51:15 GMT
ADD file:ee35e95b906b98c2d7493d8c365bf5aaf351251abce763f9be2d9fa6cc541aaf in / 
# Tue, 04 Oct 2022 23:51:15 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:18:49 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 05 Oct 2022 14:19:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:19:08 GMT
ENV JAVA_VERSION=8.0.7.16
# Wed, 05 Oct 2022 14:21:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bb34f647a77ae43611dab3a447da447686352da5426baaff26c22a465dfe40c0';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='b8c35301b56fde151b14e1bfb1374f579f5a0ed361d6ebc7ffff5f82eb563344';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='79fde4473b2c489278fdef105bf69097f1f1a0d54d75a59d24008773b512339b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f1989ee7f41d8d697e880dea74f94133841c2f59ded5c9dd551a26b87f4d36cf';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='eb1cd5b6bf532f10558e7067768d14884d9fce375d2782f91b2218365152bc42';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 05 Oct 2022 14:21:59 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:6d1a231d13b300fc73c20f074f3accd74dcff41afd006c272719fdf8cf9be075`  
		Last Modified: Tue, 04 Oct 2022 23:52:01 GMT  
		Size: 27.2 MB (27165243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766942147a0b9643dde5105adf200582201a20a0ef3ad86d7136e55632dd694c`  
		Last Modified: Wed, 05 Oct 2022 14:22:30 GMT  
		Size: 3.0 MB (2983220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a590bea68a831fcee3304072a3678ee2f07e2a7e0a23a0c1654611eba1d4b2f9`  
		Last Modified: Wed, 05 Oct 2022 14:23:20 GMT  
		Size: 154.5 MB (154503954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:eb29bbde87c9e14c155ba0ce91c6ad689744991991a51b31b018e01b88fda823
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.8 MB (199803701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392236ab71cfb2c0a19c87dba93e852e4bc5130f5ea9e980b0d98ca607103e28`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 10:51:52 GMT
ADD file:d93b8e74342ae6048a42c90c30192dd384e92b697ad4d8d5944868e03325820c in / 
# Wed, 05 Oct 2022 10:51:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 20:30:38 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 05 Oct 2022 20:30:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 20:30:56 GMT
ENV JAVA_VERSION=8.0.7.16
# Wed, 05 Oct 2022 20:38:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bb34f647a77ae43611dab3a447da447686352da5426baaff26c22a465dfe40c0';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='b8c35301b56fde151b14e1bfb1374f579f5a0ed361d6ebc7ffff5f82eb563344';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='79fde4473b2c489278fdef105bf69097f1f1a0d54d75a59d24008773b512339b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f1989ee7f41d8d697e880dea74f94133841c2f59ded5c9dd551a26b87f4d36cf';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='eb1cd5b6bf532f10558e7067768d14884d9fce375d2782f91b2218365152bc42';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 05 Oct 2022 20:38:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:faece833463c99bd10748da29171f2d588a627912f7bbb982b3ca4512dd39eed`  
		Last Modified: Wed, 05 Oct 2022 10:54:03 GMT  
		Size: 30.4 MB (30442565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52af0b72f683bca4c76215658777957eba73fde39f2157d70f361b51f1e4c42`  
		Last Modified: Wed, 05 Oct 2022 20:38:46 GMT  
		Size: 3.1 MB (3075970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6063a757f44e967a2c39a4720f2475e7d496a1b04bdb493ecf2955b7061e4a2`  
		Last Modified: Wed, 05 Oct 2022 20:40:02 GMT  
		Size: 166.3 MB (166285166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:741c0cc42327a190e5995b5dc297c1f7c4e569a778cf2aa7d83a07d4ff32476c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.8 MB (184811184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3fcddc077c3020a957cccd488a295888e7b4ccecb693186e3c2c10168a2e882`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:52:31 GMT
ADD file:29c2a2a72a634a5f21c2f37cfd38da282528b75f75124d04e56a2f86f2e64121 in / 
# Tue, 04 Oct 2022 23:52:34 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:07:07 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 05 Oct 2022 08:07:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:07:26 GMT
ENV JAVA_VERSION=8.0.7.16
# Wed, 05 Oct 2022 08:10:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bb34f647a77ae43611dab3a447da447686352da5426baaff26c22a465dfe40c0';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='b8c35301b56fde151b14e1bfb1374f579f5a0ed361d6ebc7ffff5f82eb563344';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='79fde4473b2c489278fdef105bf69097f1f1a0d54d75a59d24008773b512339b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f1989ee7f41d8d697e880dea74f94133841c2f59ded5c9dd551a26b87f4d36cf';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='eb1cd5b6bf532f10558e7067768d14884d9fce375d2782f91b2218365152bc42';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 05 Oct 2022 08:10:52 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:f41c9e2df5b8fcd28b58de30866b751466a2cbad7eb8f43e02d799439fb377cf`  
		Last Modified: Tue, 04 Oct 2022 23:54:09 GMT  
		Size: 25.4 MB (25370644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42b030bfbe7d3d22ba17686023d66542eece08a7b4916da1aa44dbd0fdc84f3`  
		Last Modified: Wed, 05 Oct 2022 08:11:26 GMT  
		Size: 2.7 MB (2671847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecefa2f8f5a24ca441bfef6e86f26f96eb27ac714576f1f61fb33d8c2fa796c`  
		Last Modified: Wed, 05 Oct 2022 08:12:08 GMT  
		Size: 156.8 MB (156768693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
