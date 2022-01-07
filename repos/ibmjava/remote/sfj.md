## `ibmjava:sfj`

```console
$ docker pull ibmjava@sha256:eac0133e24d46d67655185f90e6bd4de6e9a9f994efcd909c8945f0d35776d87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:3d049855508f870d4f80c4085f9b925ed48e8d5e381bbe2fdbf2a8346207fa50
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94218176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4e89488895d6767a805828adf4f820627e62baac8888969e8185b6049500b56`
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
# Mon, 29 Nov 2021 21:17:09 GMT
ENV JAVA_VERSION=8.0.7.0
# Mon, 29 Nov 2021 21:18:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='8110bd65dc4139d169bd3ca1494e2d34e7b57729634a2e4cdbfc3ed86c10cb37';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='dccd32d60bb77d37fd0feb4f78ee08f55002f2a5691dcd810bc87cf1a4a5d3a6';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='84aa2438d229261e841ba73d1d20817725b370b01c2580b9ceeda9479b54d0fe';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='114414f4b2e2405f9248a1e61b45b0835fe6773a89bc5aa1407e1c042c228636';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='9edb12668be67fcdf9e01160e71ff930677c2ceba22d5afeb0a3757908b8bd4f';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Mon, 29 Nov 2021 21:18:56 GMT
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
	-	`sha256:6e7ff3d71eda8d8c54f720efdc7b431d921eeae54b3d1aac71984e863dfaa942`  
		Last Modified: Mon, 29 Nov 2021 21:22:11 GMT  
		Size: 64.6 MB (64553229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:510b5c2fb56f76b825896efbcb7bda47c6235a9b501c7de5729f66a50241d026
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.1 MB (94091303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7744bef03e03512b006cac87e5b0bbba3a929f26d811e22411d3a956dff61a9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:39:03 GMT
ADD file:4992040d291a9a6b53435279ff532c15e004fd7c7b35aa4783850a06ccff0694 in / 
# Fri, 07 Jan 2022 01:39:04 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 01:55:19 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 01:55:38 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 01:55:38 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 01:56:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='8110bd65dc4139d169bd3ca1494e2d34e7b57729634a2e4cdbfc3ed86c10cb37';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='dccd32d60bb77d37fd0feb4f78ee08f55002f2a5691dcd810bc87cf1a4a5d3a6';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='84aa2438d229261e841ba73d1d20817725b370b01c2580b9ceeda9479b54d0fe';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='114414f4b2e2405f9248a1e61b45b0835fe6773a89bc5aa1407e1c042c228636';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='9edb12668be67fcdf9e01160e71ff930677c2ceba22d5afeb0a3757908b8bd4f';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 01:56:59 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:cd8c855b84a6297384d4a364fec672137f3aef84749b319ee5158b568545eb0f`  
		Last Modified: Fri, 07 Jan 2022 01:39:50 GMT  
		Size: 27.2 MB (27156435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2117a5cceef36b33a766d89032a5ed9031aa846b7f4aa20b30313c553fc2f481`  
		Last Modified: Fri, 07 Jan 2022 01:58:17 GMT  
		Size: 3.0 MB (2988908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac46c1abc3febef22faf7ef3496ce065ef4de7731d4d57b75eade31c053b9ea`  
		Last Modified: Fri, 07 Jan 2022 01:58:53 GMT  
		Size: 63.9 MB (63945960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:b8878f4fee1c538cb1369dd5089c41f1cf64c419083b6179c80f5b0eadd839a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.3 MB (98279235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b2e66b9ed71fbd32bd93c5dd99a846eef8dde15e3378d0655c5058ee8d7c302`
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
# Mon, 29 Nov 2021 21:04:52 GMT
ENV JAVA_VERSION=8.0.7.0
# Mon, 29 Nov 2021 21:06:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='8110bd65dc4139d169bd3ca1494e2d34e7b57729634a2e4cdbfc3ed86c10cb37';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='dccd32d60bb77d37fd0feb4f78ee08f55002f2a5691dcd810bc87cf1a4a5d3a6';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='84aa2438d229261e841ba73d1d20817725b370b01c2580b9ceeda9479b54d0fe';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='114414f4b2e2405f9248a1e61b45b0835fe6773a89bc5aa1407e1c042c228636';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='9edb12668be67fcdf9e01160e71ff930677c2ceba22d5afeb0a3757908b8bd4f';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Mon, 29 Nov 2021 21:06:48 GMT
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
	-	`sha256:05ee8b6cdd34820c6051ee860c90f1abb8dd605202da56561fc24e58b046b5b8`  
		Last Modified: Mon, 29 Nov 2021 21:09:11 GMT  
		Size: 64.8 MB (64764734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:6baf6b313b0cfda61d8a74d7cc565703ff420fc34de4b123b14781735c029c2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.6 MB (93635740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1032a14804a4b4e452e7c88dcd58e48e44ace238045aa7c750d4c7799bf021`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:09 GMT
ADD file:caefb9be68fabe0b9b7dba683dabb869e5165a5a13534742d73a489a3712d9a9 in / 
# Fri, 07 Jan 2022 01:42:12 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:20:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 02:20:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:20:32 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 02:21:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='8110bd65dc4139d169bd3ca1494e2d34e7b57729634a2e4cdbfc3ed86c10cb37';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='dccd32d60bb77d37fd0feb4f78ee08f55002f2a5691dcd810bc87cf1a4a5d3a6';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='84aa2438d229261e841ba73d1d20817725b370b01c2580b9ceeda9479b54d0fe';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='114414f4b2e2405f9248a1e61b45b0835fe6773a89bc5aa1407e1c042c228636';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='9edb12668be67fcdf9e01160e71ff930677c2ceba22d5afeb0a3757908b8bd4f';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 02:21:54 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:7587f9252eef493a02840102ba78c74de317d3d47f6d568af5602ff6c1c54a20`  
		Last Modified: Fri, 07 Jan 2022 01:43:57 GMT  
		Size: 25.4 MB (25362136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d5d9207d0f328849a5bf2aec9290cf52dbfa8a48e3d39b130fd1471f46a16e`  
		Last Modified: Fri, 07 Jan 2022 02:23:17 GMT  
		Size: 2.7 MB (2676903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270690b604ff70add5a3faa491957cb55e4215b9d5ff72074e19d05a30de2969`  
		Last Modified: Fri, 07 Jan 2022 02:23:40 GMT  
		Size: 65.6 MB (65596701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
