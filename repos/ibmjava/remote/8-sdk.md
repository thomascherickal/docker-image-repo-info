## `ibmjava:8-sdk`

```console
$ docker pull ibmjava@sha256:a1a9924a41c76e85000979d32e1179d0dcbbbaf093e1e0ababa4b13df84c7b09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:5f8d0bc6e217ac0029f08a6911ee1cb4b5fc972df2ded230ba02ff5ced72d07a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.2 MB (195196153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c04be7aa3c51eeaef189bb8100aba4200b124978e46dbcbc3f67e6c6a3b7c78`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:55:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:55:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:55:32 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:57:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='953586dcb1870406d51fc0f346e2be062471d7dc67dce21ba2009cff0a46724f';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='09705ba9b6c53105062fd7764f9a066bfe5e2f58a64662d29c1eb030d51252e1';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e233b23f00ecda6a8e8fffe4b7c0675c3574754d300b680e70f423a60d047874';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e81cde52da8dd39160a70c98453e379f1286bb39e58f01ba94a63e45e31e2d34';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='dfc67c2861e00265140287091a713496840f5793946e087825f96c7afd4a8a50';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:57:31 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7ef5b4a4700901695d7489ffa25c9a36a0c54f7003664412a2a582dd362fa`  
		Last Modified: Fri, 01 Oct 2021 02:59:16 GMT  
		Size: 3.0 MB (2959872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d70a5bfa8e87d64a9f2b2f6fdedbe49d6f21667069866e8ba624a15c35ef98b`  
		Last Modified: Fri, 01 Oct 2021 03:00:12 GMT  
		Size: 165.5 MB (165531206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:55e510819e8889767ece5babbc8cf319de7aca7cb6404e3ebb3905f52417e0e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.9 MB (183888113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7756abf2283051a369b57422d8194fbacb7b6d17c46975bc9dacff0ee7e657b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 03:46:35 GMT
ADD file:6718b956b86d332e4a53184568ac5205e92f9edeba804c64254e3b2da6e66c72 in / 
# Fri, 01 Oct 2021 03:46:36 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:22:39 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 04:22:46 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:22:46 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 04:24:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='953586dcb1870406d51fc0f346e2be062471d7dc67dce21ba2009cff0a46724f';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='09705ba9b6c53105062fd7764f9a066bfe5e2f58a64662d29c1eb030d51252e1';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e233b23f00ecda6a8e8fffe4b7c0675c3574754d300b680e70f423a60d047874';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e81cde52da8dd39160a70c98453e379f1286bb39e58f01ba94a63e45e31e2d34';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='dfc67c2861e00265140287091a713496840f5793946e087825f96c7afd4a8a50';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 04:25:00 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:96391085795d2daa9755c58002e78a76eecf7fd57a1d8a3778e87b0079ed47e9`  
		Last Modified: Fri, 01 Oct 2021 03:47:35 GMT  
		Size: 27.2 MB (27158466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfd8a2f00fd7231d93b6eab959a6ea65acafe045c09e9e0602b1ea4293dd6c2`  
		Last Modified: Fri, 01 Oct 2021 04:25:31 GMT  
		Size: 3.0 MB (2988884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b25b2d568fc535899c14f210de6b8b399d2cc3d41fca90feab7f10fc3ae4b9`  
		Last Modified: Fri, 01 Oct 2021 04:26:36 GMT  
		Size: 153.7 MB (153740763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:13300e3b13ffc5b18ccf20b4af7712bb99d8a8fbca5227a79ee4cbe7de8d2af1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.7 MB (198692128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a05a660b4c9b5f093f8c4379e5c59aebe48f99a4bccac3342946e24e83773d94`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 06:11:59 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 06:14:53 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Sep 2021 19:44:02 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 17 Sep 2021 19:48:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='953586dcb1870406d51fc0f346e2be062471d7dc67dce21ba2009cff0a46724f';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='09705ba9b6c53105062fd7764f9a066bfe5e2f58a64662d29c1eb030d51252e1';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e233b23f00ecda6a8e8fffe4b7c0675c3574754d300b680e70f423a60d047874';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e81cde52da8dd39160a70c98453e379f1286bb39e58f01ba94a63e45e31e2d34';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='dfc67c2861e00265140287091a713496840f5793946e087825f96c7afd4a8a50';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 17 Sep 2021 19:48:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a83a649f63bfaad86f8628a777426148c29a6119ce301cd77dbdf1d4c48ddcb`  
		Last Modified: Tue, 31 Aug 2021 06:19:28 GMT  
		Size: 3.1 MB (3084352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6cdd2754d3060e4d16ef0d9b1bb817e8e074f5f5d320262e6947293a7c1af`  
		Last Modified: Fri, 17 Sep 2021 19:50:11 GMT  
		Size: 165.2 MB (165170018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:43a95f5511e91c9a45566304e13c1180d0be402e27439f1f6483f6f056cf49ce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.7 MB (183716995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6da8fa40e0655ce5db4c8f7affec58fdcf9c6131696fffd12c900e2a3cb09637`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:23:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:23:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:37 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:25:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='953586dcb1870406d51fc0f346e2be062471d7dc67dce21ba2009cff0a46724f';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='09705ba9b6c53105062fd7764f9a066bfe5e2f58a64662d29c1eb030d51252e1';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e233b23f00ecda6a8e8fffe4b7c0675c3574754d300b680e70f423a60d047874';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e81cde52da8dd39160a70c98453e379f1286bb39e58f01ba94a63e45e31e2d34';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='dfc67c2861e00265140287091a713496840f5793946e087825f96c7afd4a8a50';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:25:51 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf425722012c2264c66ba97a53ff25a2f196330fbcc0872474e5e4562fa95f0`  
		Last Modified: Fri, 01 Oct 2021 02:27:43 GMT  
		Size: 2.7 MB (2676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3d9e09f0d1a147988e4b3a76835bc5965456062e5ded148222a25944881787`  
		Last Modified: Fri, 01 Oct 2021 02:28:26 GMT  
		Size: 155.7 MB (155677712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
