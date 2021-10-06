## `ibmjava:8-sfj`

```console
$ docker pull ibmjava@sha256:ba2dfd6e4fa5cf63313dbf8eab5af588bfe58b9f92c18c49d177f0bb9465c9e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:04f9a05119a8931e696fe1b064851c6f1af2a94b13102fc34d056fe823648487
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (93956348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd99b5b3882c2907cffafcec2938e25265dee3f3ecec05232135e5145a3b56bd`
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
# Fri, 01 Oct 2021 02:56:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='aee78edcb2b1eed2e89b60ecfd787c77cc86e1fea646d06e5064f33615379bef';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='1a7c2738e1843d3bc117168ceb8f2969592ff75488d381aa380d647892603204';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f0872801318d37b29f962c4e1ff7f4ea3b201bd401f68b41f1f670b2059c58aa';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='6f8e7f2dfc04a4fddf6ef46640791048d9b87d437cd5f724dbf90f1e5ed38f56';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='1a16198540ec2b521d8290bdb37f4ed9848e1d85c6f20c4ef4aa9ae8d4d8cb1e';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:56:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:853b1d3af684da44d00cddd3eab52b1432ba6800c6c6cc43b6b972d599c93ab2`  
		Last Modified: Fri, 01 Oct 2021 02:59:47 GMT  
		Size: 64.3 MB (64291401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:ee16f8052dc2ea75faba142ecb39deb53a876b2dc7a41fcb568471bd6fcdc8b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93838990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2630a28e01ad1068fe9f5f6ad3472e91ee472299f92eb10cb87e40a01b12c1a0`
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
# Fri, 01 Oct 2021 04:24:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='aee78edcb2b1eed2e89b60ecfd787c77cc86e1fea646d06e5064f33615379bef';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='1a7c2738e1843d3bc117168ceb8f2969592ff75488d381aa380d647892603204';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f0872801318d37b29f962c4e1ff7f4ea3b201bd401f68b41f1f670b2059c58aa';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='6f8e7f2dfc04a4fddf6ef46640791048d9b87d437cd5f724dbf90f1e5ed38f56';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='1a16198540ec2b521d8290bdb37f4ed9848e1d85c6f20c4ef4aa9ae8d4d8cb1e';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 04:24:11 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:ba3b102834bc1223f1977f59631ff70eb76e73905de447bea3f7e4cae467ae32`  
		Last Modified: Fri, 01 Oct 2021 04:26:08 GMT  
		Size: 63.7 MB (63691640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:c7ef9c9272c2dbe655568c892531e1414892df88fcc37819993bedd19c5ee258
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98008256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b05d4a27df24785361ed10ea0da0e2455050df0ba0da17001ddd8a9f0aed2a88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:55:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Oct 2021 17:56:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:56:16 GMT
ENV JAVA_VERSION=8.0.6.36
# Wed, 06 Oct 2021 17:58:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='aee78edcb2b1eed2e89b60ecfd787c77cc86e1fea646d06e5064f33615379bef';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='1a7c2738e1843d3bc117168ceb8f2969592ff75488d381aa380d647892603204';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f0872801318d37b29f962c4e1ff7f4ea3b201bd401f68b41f1f670b2059c58aa';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='6f8e7f2dfc04a4fddf6ef46640791048d9b87d437cd5f724dbf90f1e5ed38f56';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='1a16198540ec2b521d8290bdb37f4ed9848e1d85c6f20c4ef4aa9ae8d4d8cb1e';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Oct 2021 17:59:01 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6e130fd3d09fd3fe6d741e0fa3f77120aa82717cf6d0a1cb49439939243a6`  
		Last Modified: Wed, 06 Oct 2021 18:04:08 GMT  
		Size: 3.1 MB (3081580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534c645d749f4cfda9e521aad595946b025f3e827c3cd5d4b4eff168548ba8c0`  
		Last Modified: Wed, 06 Oct 2021 18:04:47 GMT  
		Size: 64.5 MB (64493755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:7d37e43ef2352a88cbceb2754a4a78176f9f2a115bcd16ce86b53210cce6e875
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93378310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bda08838977c9da09fad39659c7c4edf1d25c61811d7d9a67e548b0b58e0d243`
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
# Fri, 01 Oct 2021 02:24:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='aee78edcb2b1eed2e89b60ecfd787c77cc86e1fea646d06e5064f33615379bef';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='1a7c2738e1843d3bc117168ceb8f2969592ff75488d381aa380d647892603204';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f0872801318d37b29f962c4e1ff7f4ea3b201bd401f68b41f1f670b2059c58aa';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='6f8e7f2dfc04a4fddf6ef46640791048d9b87d437cd5f724dbf90f1e5ed38f56';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='1a16198540ec2b521d8290bdb37f4ed9848e1d85c6f20c4ef4aa9ae8d4d8cb1e';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:24:58 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:435a2c3b6b4b4ccfba1dc3df9b876829bd0f62385efb5cfdc591c944026b3d91`  
		Last Modified: Fri, 01 Oct 2021 02:28:09 GMT  
		Size: 65.3 MB (65339027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
