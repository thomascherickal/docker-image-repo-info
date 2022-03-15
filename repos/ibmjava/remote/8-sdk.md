## `ibmjava:8-sdk`

```console
$ docker pull ibmjava@sha256:7c0ffcd0a9030121123c32ed94cbd05474a7234f7a62575fe3ca68370172fe7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:7aa9ebb87c1d0344e86c072c39d282a6d4fabdfd8b1bf57fdf87549f57fab0e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.6 MB (195614371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da8e12f4cc01c6974110f8c354b70e82e5cfd7db63c9e7f8b3b06b7b91acda8b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:25 GMT
ADD file:dee0aa8497bd26ca41dffa17adff99be2523f66f9b2c557ba9ad2388ed052dca in / 
# Thu, 03 Mar 2022 20:19:25 GMT
CMD ["bash"]
# Mon, 14 Mar 2022 18:08:29 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 14 Mar 2022 18:08:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Mon, 14 Mar 2022 18:08:49 GMT
ENV JAVA_VERSION=8.0.7.5
# Mon, 14 Mar 2022 18:10:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='92780907321f498f161e79e44adc2b7d5c2393dd2f19eb1573c82f3aa332f614';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='9a20d1fa4088717d880c129d75e290b53db6491ef05aa3aa96ada94274cb97b2';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0457ef521004b5ffbe5b96d3383f4632497990bbad54d91497b8558672d3bc3b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='7ff867607d7e5d8102e79416f6a844b095ffdc5bbc7d29db5e8f5c999127d262';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='9f254c353ac53073f08e4969ad33b8f911f88c11472309ba9c0b150ef4b420b9';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Mon, 14 Mar 2022 18:10:48 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:cf06a7c3161117888114e7e91dbd21915efae33c2dbfb086380f7b21946d6e59`  
		Last Modified: Thu, 03 Mar 2022 20:20:28 GMT  
		Size: 26.7 MB (26708326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf7401dcb52ce7bb3a51e6367cb30dcb4167c78f4ceb8611d1d515c1248fb2d`  
		Last Modified: Mon, 14 Mar 2022 18:11:11 GMT  
		Size: 3.0 MB (2959827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea38094917655b88f5d543fd478f385923ea6da2086084344f75c86bd9ccb5f`  
		Last Modified: Mon, 14 Mar 2022 18:12:03 GMT  
		Size: 165.9 MB (165946218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:3b78580cf6a4efa0930b827f6af1c1ddd715e9c6080d05b4531484ad43910f3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.2 MB (184221157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2d373376e6a67d5beacb9035311ef9b758837804679276b88d5e26a89499370`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 03 Mar 2022 20:18:47 GMT
ADD file:2ae34e7bffe3a59f3167a286025a093609188772be7b14601867a334bb3c0166 in / 
# Thu, 03 Mar 2022 20:18:48 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 20:45:10 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 03 Mar 2022 20:45:17 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 20:45:17 GMT
ENV JAVA_VERSION=8.0.7.5
# Thu, 03 Mar 2022 20:47:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='92780907321f498f161e79e44adc2b7d5c2393dd2f19eb1573c82f3aa332f614';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='9a20d1fa4088717d880c129d75e290b53db6491ef05aa3aa96ada94274cb97b2';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0457ef521004b5ffbe5b96d3383f4632497990bbad54d91497b8558672d3bc3b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='7ff867607d7e5d8102e79416f6a844b095ffdc5bbc7d29db5e8f5c999127d262';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='9f254c353ac53073f08e4969ad33b8f911f88c11472309ba9c0b150ef4b420b9';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 03 Mar 2022 20:47:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:250799bdfa37968bdaf47cc4d86f759e4e574d5e795f888e42c66ec0b7e92034`  
		Last Modified: Thu, 03 Mar 2022 20:19:35 GMT  
		Size: 27.2 MB (27161874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6497c383d83f87f745e318bca389751c8234e755523898bf644cde419db8ef`  
		Last Modified: Thu, 03 Mar 2022 20:47:47 GMT  
		Size: 3.0 MB (2988885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b4bd88bb652b695a9bcbbb60ffd41a1c7ee135e61cd3f922601fa6673db634`  
		Last Modified: Thu, 03 Mar 2022 20:48:48 GMT  
		Size: 154.1 MB (154070398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:804aadd306cf1d7e66080eb881a71e670cd9ee89ac5943c796895c578b008da2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.1 MB (199106646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f125377aa95474208979b1b3f1a0757bf5966376bf8b0a88ef6967bb550cf2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Feb 2022 03:49:58 GMT
ADD file:19b6b516bfde37805273abae0012aaceb45030dcc0c1dbc11828a4dfa6549c29 in / 
# Wed, 02 Feb 2022 03:50:03 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:01:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 06:01:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 18:17:17 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 23 Feb 2022 18:21:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='92780907321f498f161e79e44adc2b7d5c2393dd2f19eb1573c82f3aa332f614';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='9a20d1fa4088717d880c129d75e290b53db6491ef05aa3aa96ada94274cb97b2';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0457ef521004b5ffbe5b96d3383f4632497990bbad54d91497b8558672d3bc3b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='7ff867607d7e5d8102e79416f6a844b095ffdc5bbc7d29db5e8f5c999127d262';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='9f254c353ac53073f08e4969ad33b8f911f88c11472309ba9c0b150ef4b420b9';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 23 Feb 2022 18:21:39 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:1dc99fe180768d17487534d27fca7d2aea3e7473c284314a65af7be77144eeaa`  
		Last Modified: Wed, 02 Feb 2022 03:52:51 GMT  
		Size: 30.4 MB (30437685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e519c40c78b488d71991dd0054bffe8260611286580cb61463ffb1d4b81bb2`  
		Last Modified: Wed, 02 Feb 2022 06:05:57 GMT  
		Size: 3.1 MB (3081867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb74ecbcc80d94c14b6b869cb3eddcfabd197a22dde414446a12e950fc157c84`  
		Last Modified: Wed, 23 Feb 2022 18:23:37 GMT  
		Size: 165.6 MB (165587094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:1ef08f3d6e3c697f98c72012051f6986a4c4dcf03634257129dac547725494bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184134273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba8122502d4e9603d855968b517e2152d75f0a55b7d64dff7e68b2c93248d6a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 03 Mar 2022 19:41:41 GMT
ADD file:84b8165a5044433cc2f9fdf9670d391f085aad3799d5e6dae035f8338dbe6081 in / 
# Thu, 03 Mar 2022 19:41:44 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 20:45:56 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 03 Mar 2022 20:46:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 20:46:03 GMT
ENV JAVA_VERSION=8.0.7.5
# Thu, 03 Mar 2022 20:48:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='92780907321f498f161e79e44adc2b7d5c2393dd2f19eb1573c82f3aa332f614';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='9a20d1fa4088717d880c129d75e290b53db6491ef05aa3aa96ada94274cb97b2';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0457ef521004b5ffbe5b96d3383f4632497990bbad54d91497b8558672d3bc3b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='7ff867607d7e5d8102e79416f6a844b095ffdc5bbc7d29db5e8f5c999127d262';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='9f254c353ac53073f08e4969ad33b8f911f88c11472309ba9c0b150ef4b420b9';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 03 Mar 2022 20:48:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:084e045c78b3a9e38ef6caaf47c3ef1c3d672d3cc2e60543ae9629511a5e1c8b`  
		Last Modified: Thu, 03 Mar 2022 19:43:09 GMT  
		Size: 25.4 MB (25365258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdf7842165599d19086acd25ada4ee293ff50581268df996a4b6e2c99d31bcf`  
		Last Modified: Thu, 03 Mar 2022 20:48:48 GMT  
		Size: 2.7 MB (2676824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27663c2f110152168d2e6ec76ea5275eb0d3c2d8964c899f7edb7ed525bdda23`  
		Last Modified: Thu, 03 Mar 2022 20:49:30 GMT  
		Size: 156.1 MB (156092191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
