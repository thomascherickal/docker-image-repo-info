## `maven:ibmjava`

```console
$ docker pull maven@sha256:05b941841c98d4fbfc9c2a8c715174c6f560c0f77bd439311f8dcb5b4aec7d7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `maven:ibmjava` - linux; amd64

```console
$ docker pull maven@sha256:edeca1d266a4d0cd5fb495495cf2c384fe4fa2bcbd2d5036cb453fce3ac4d695
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236113929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a811cf206616322d965e937d84514eac49cd3df9e74fcdd4c65477e6825bce2d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:36 GMT
ADD file:c6039a4f004b6b6c2e4c281a228d64d8410cb9fdf0c67776f84bb173d3522be1 in / 
# Wed, 02 Feb 2022 02:14:36 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:40:26 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 03:40:35 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 18:19:41 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 23 Feb 2022 18:22:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='92780907321f498f161e79e44adc2b7d5c2393dd2f19eb1573c82f3aa332f614';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='9a20d1fa4088717d880c129d75e290b53db6491ef05aa3aa96ada94274cb97b2';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0457ef521004b5ffbe5b96d3383f4632497990bbad54d91497b8558672d3bc3b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='7ff867607d7e5d8102e79416f6a844b095ffdc5bbc7d29db5e8f5c999127d262';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='9f254c353ac53073f08e4969ad33b8f911f88c11472309ba9c0b150ef4b420b9';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 23 Feb 2022 18:22:47 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 23 Feb 2022 18:56:53 GMT
RUN apt-get update && apt-get install -y curl
# Wed, 23 Feb 2022 18:56:54 GMT
ARG MAVEN_VERSION=3.8.4
# Wed, 23 Feb 2022 18:56:54 GMT
ARG USER_HOME_DIR=/root
# Wed, 23 Feb 2022 18:56:54 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Wed, 23 Feb 2022 18:56:54 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Wed, 23 Feb 2022 18:56:57 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 23 Feb 2022 18:56:57 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 23 Feb 2022 18:56:57 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 23 Feb 2022 18:56:57 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 23 Feb 2022 18:56:58 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 23 Feb 2022 18:56:58 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 23 Feb 2022 18:56:58 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:68e7bb398b9ff421236990bfeaf5c1feab26c590eed93489e245375c23551e2a`  
		Last Modified: Sat, 29 Jan 2022 14:35:20 GMT  
		Size: 26.7 MB (26708066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fb07417efc9ce7b84eb9ed465e87c936352af2a77456046d4e4c6f7f3e7a57`  
		Last Modified: Wed, 02 Feb 2022 03:42:54 GMT  
		Size: 3.0 MB (2959756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ab40dda7cb116b48792248dd7c2b107ae062ae4685a6b876cf27940724cfe5`  
		Last Modified: Wed, 23 Feb 2022 18:27:03 GMT  
		Size: 165.9 MB (165946404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426c50bcdaae9f2ef61bfbc3b4fd0350b539f438468252ce7f8b7266b12c277e`  
		Last Modified: Wed, 23 Feb 2022 18:59:27 GMT  
		Size: 31.4 MB (31388676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f381af8d1b7c86e77fb579f8f3812066e1e6cd6b08ef510ed90afb5a6ec10012`  
		Last Modified: Wed, 23 Feb 2022 18:59:25 GMT  
		Size: 9.1 MB (9109815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dd2e1a295a753abba7149232aaa690b84cb65bb20ac8afbae98282e3f882e3`  
		Last Modified: Wed, 23 Feb 2022 18:59:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211865725e581d0e8e8e269b3bf69fcc1f2020555aaee3dd3fbf718e1a822e6b`  
		Last Modified: Wed, 23 Feb 2022 18:59:24 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; 386

```console
$ docker pull maven@sha256:582baa2590d2ab312b7b6adb09011c735098f35195345cbbd67d6c4ec59fcbbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.2 MB (221227988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07b568babdd168ef599883a64c22fd604c493da6a73ba9be3e44c9d0f12ea756`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 02 Feb 2022 01:39:15 GMT
ADD file:41a670fdf6e067377f3e555206d80e9dddb0d180cd7493802d3989acb2c1b573 in / 
# Wed, 02 Feb 2022 01:39:16 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 01:55:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 01:56:00 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 18:38:41 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 23 Feb 2022 18:40:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='92780907321f498f161e79e44adc2b7d5c2393dd2f19eb1573c82f3aa332f614';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='9a20d1fa4088717d880c129d75e290b53db6491ef05aa3aa96ada94274cb97b2';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0457ef521004b5ffbe5b96d3383f4632497990bbad54d91497b8558672d3bc3b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='7ff867607d7e5d8102e79416f6a844b095ffdc5bbc7d29db5e8f5c999127d262';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='9f254c353ac53073f08e4969ad33b8f911f88c11472309ba9c0b150ef4b420b9';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 23 Feb 2022 18:40:48 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 23 Feb 2022 18:58:03 GMT
RUN apt-get update && apt-get install -y curl
# Wed, 23 Feb 2022 18:58:03 GMT
ARG MAVEN_VERSION=3.8.4
# Wed, 23 Feb 2022 18:58:04 GMT
ARG USER_HOME_DIR=/root
# Wed, 23 Feb 2022 18:58:04 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Wed, 23 Feb 2022 18:58:04 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Wed, 23 Feb 2022 18:58:10 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 23 Feb 2022 18:58:11 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 23 Feb 2022 18:58:11 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 23 Feb 2022 18:58:11 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 23 Feb 2022 18:58:12 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 23 Feb 2022 18:58:12 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 23 Feb 2022 18:58:12 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:783703cdc79d2cd178a6be62b27388915bbc0dabf13db414d7ee577514c92adf`  
		Last Modified: Wed, 02 Feb 2022 01:40:03 GMT  
		Size: 27.2 MB (27161586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944419a0797263cb1168e0715821610315031f2aef101b1e93ceca4cafaa3636`  
		Last Modified: Wed, 02 Feb 2022 01:58:34 GMT  
		Size: 3.0 MB (2988866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc6c13d44e720143daa3e86ce77b1d0cd05694d3f8612ffaf85ec3d1e914418`  
		Last Modified: Wed, 23 Feb 2022 18:42:16 GMT  
		Size: 154.1 MB (154070525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40955037a5e78680fa00fbcc87c1c56a85a68b565525a2295a21dfe9dca98306`  
		Last Modified: Wed, 23 Feb 2022 18:58:42 GMT  
		Size: 27.9 MB (27895960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a1f2a30a891036f3fa1f5c6b4370f9d46ab66a6feededdd88bcfd66b5b7cb4`  
		Last Modified: Wed, 23 Feb 2022 18:58:40 GMT  
		Size: 9.1 MB (9109833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06752867a6583c598de84f6cc2e3eab6f65f700ba77b5af03f314cb3bf819e29`  
		Last Modified: Wed, 23 Feb 2022 18:58:39 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aae578912540bc7b9aa4b63b05568ea830f453d6dad7f899a85fa0ef404a8a7`  
		Last Modified: Wed, 23 Feb 2022 18:58:38 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; ppc64le

```console
$ docker pull maven@sha256:d61d3d6b37a5f07175e395da8cc8e193f11286918a080167c4d8ffe2bb3b6708
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.4 MB (233399487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d6a74552a20a95cb0f62414ad385cf5e4538475af52cc549e4cbfeec9129b27`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

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
# Wed, 23 Feb 2022 18:43:05 GMT
RUN apt-get update && apt-get install -y curl
# Wed, 23 Feb 2022 18:43:18 GMT
ARG MAVEN_VERSION=3.8.4
# Wed, 23 Feb 2022 18:43:26 GMT
ARG USER_HOME_DIR=/root
# Wed, 23 Feb 2022 18:43:40 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Wed, 23 Feb 2022 18:43:59 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Wed, 23 Feb 2022 18:44:24 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 23 Feb 2022 18:44:35 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 23 Feb 2022 18:44:42 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 23 Feb 2022 18:44:45 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 23 Feb 2022 18:44:49 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 23 Feb 2022 18:45:03 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 23 Feb 2022 18:45:18 GMT
CMD ["mvn"]
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
	-	`sha256:76d444ad408367a2d9613b22c26d4975b9a2308293e18af156793eaacfb46fff`  
		Last Modified: Wed, 23 Feb 2022 18:47:14 GMT  
		Size: 25.2 MB (25181804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea0175b914f6bccd96aea3dc76e5e6a6060eb2bbf9fa4e9b9f84ee477856cad`  
		Last Modified: Wed, 23 Feb 2022 18:47:12 GMT  
		Size: 9.1 MB (9109816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4057b97ecd83d6b9484ba6e03fc84cd5f9a1d816778aceaf08f0c508a6fef6bc`  
		Last Modified: Wed, 23 Feb 2022 18:47:10 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e675373320d60fc14bbaff279251d1967c0adef0969b3c2598730b91c6b426`  
		Last Modified: Wed, 23 Feb 2022 18:47:10 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; s390x

```console
$ docker pull maven@sha256:f04a5a4acd0ed17cecc099ce1d6fe40f4467076365a2d769b8ae013fb5fa0233
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216419405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:328b0e4bca31c8912732d481612e44424253ea589c23d40c7a9b6c4c2e4a2383`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:03 GMT
ADD file:3fe2ce9d5d8932ed39dc2c73abff4b15e244fb1e7eb456de0a05df07ede3bf39 in / 
# Wed, 02 Feb 2022 01:42:07 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:39:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 02:39:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 18:41:31 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 23 Feb 2022 18:43:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='92780907321f498f161e79e44adc2b7d5c2393dd2f19eb1573c82f3aa332f614';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='9a20d1fa4088717d880c129d75e290b53db6491ef05aa3aa96ada94274cb97b2';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0457ef521004b5ffbe5b96d3383f4632497990bbad54d91497b8558672d3bc3b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='7ff867607d7e5d8102e79416f6a844b095ffdc5bbc7d29db5e8f5c999127d262';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='9f254c353ac53073f08e4969ad33b8f911f88c11472309ba9c0b150ef4b420b9';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 23 Feb 2022 18:43:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 23 Feb 2022 20:27:48 GMT
RUN apt-get update && apt-get install -y curl
# Wed, 23 Feb 2022 20:27:49 GMT
ARG MAVEN_VERSION=3.8.4
# Wed, 23 Feb 2022 20:27:49 GMT
ARG USER_HOME_DIR=/root
# Wed, 23 Feb 2022 20:27:49 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Wed, 23 Feb 2022 20:27:50 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Wed, 23 Feb 2022 20:27:54 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 23 Feb 2022 20:27:54 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 23 Feb 2022 20:27:54 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 23 Feb 2022 20:27:55 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 23 Feb 2022 20:27:55 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 23 Feb 2022 20:27:55 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 23 Feb 2022 20:27:55 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:cf002da3924024b39105dcc613288421b394e45e04d7a3c245ce5dcaf544dd98`  
		Last Modified: Wed, 02 Feb 2022 01:43:50 GMT  
		Size: 25.4 MB (25364307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bcdb503991176c9486c76e56946053a4588fc20649c5465c056a465c592dee`  
		Last Modified: Wed, 02 Feb 2022 02:42:23 GMT  
		Size: 2.7 MB (2676856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a31b9ce4783fc87742aae021185eb658e8d2a022d9f39142857a577a7f819f`  
		Last Modified: Wed, 23 Feb 2022 18:44:57 GMT  
		Size: 156.1 MB (156092272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846ca0b3b79798ebed299110bb75633dac153186a4f1c9d7e1ee94fe7d0654f9`  
		Last Modified: Wed, 23 Feb 2022 20:29:18 GMT  
		Size: 23.2 MB (23174930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae6f8b02188733cdaa3b1a1289b4a3d04662476270be22032a15d77c58abda8`  
		Last Modified: Wed, 23 Feb 2022 20:29:16 GMT  
		Size: 9.1 MB (9109825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45083bb103e7d6896d22891efb4088114e507a9697a3d25d2a925a2878677782`  
		Last Modified: Wed, 23 Feb 2022 20:29:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf5223bd508f5d69378aa1a25984db828e1b8ae0117734bb8633a12e7a89a6`  
		Last Modified: Wed, 23 Feb 2022 20:29:16 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
