## `maven:ibmjava`

```console
$ docker pull maven@sha256:1fffdcccec80b0cd5cb29e68ef7b419f4d55d6224a57770066cf2cdb2540f9f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `maven:ibmjava` - linux; amd64

```console
$ docker pull maven@sha256:2b852b8f90d5c509afe3e8fe803127d07bee19fb57201bc8ed283377b144422f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.1 MB (238095973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec6a8594b116b72772ec6b4e063592d006f645718262ae58481d23db75232f75`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:19:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 06 Sep 2022 20:19:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Sep 2022 00:41:44 GMT
ENV JAVA_VERSION=8.0.7.16
# Wed, 28 Sep 2022 00:44:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bb34f647a77ae43611dab3a447da447686352da5426baaff26c22a465dfe40c0';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='b8c35301b56fde151b14e1bfb1374f579f5a0ed361d6ebc7ffff5f82eb563344';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='79fde4473b2c489278fdef105bf69097f1f1a0d54d75a59d24008773b512339b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f1989ee7f41d8d697e880dea74f94133841c2f59ded5c9dd551a26b87f4d36cf';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='eb1cd5b6bf532f10558e7067768d14884d9fce375d2782f91b2218365152bc42';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 28 Sep 2022 00:44:43 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 28 Sep 2022 01:30:41 GMT
RUN apt-get update && apt-get install -y curl
# Wed, 28 Sep 2022 01:30:42 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 28 Sep 2022 01:30:42 GMT
ARG USER_HOME_DIR=/root
# Wed, 28 Sep 2022 01:30:42 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 28 Sep 2022 01:30:42 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 28 Sep 2022 01:30:45 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 28 Sep 2022 01:30:45 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 28 Sep 2022 01:30:45 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 28 Sep 2022 01:30:45 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 28 Sep 2022 01:30:46 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 28 Sep 2022 01:30:46 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 28 Sep 2022 01:30:46 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666a953ef9ff3115b0bc42a84f4510585612e4f86332b434b2a5e8382004df31`  
		Last Modified: Tue, 06 Sep 2022 20:22:22 GMT  
		Size: 3.0 MB (2957819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4a8cd9063f80a8d4c89f15af36a2a2e3f5be2577ef20766810aec5447a1bcf`  
		Last Modified: Wed, 28 Sep 2022 00:45:57 GMT  
		Size: 166.5 MB (166497648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15747344ef482e31aca5edd5c3acd3471cd0c064cbba4e6a60648decccab74c6`  
		Last Modified: Wed, 28 Sep 2022 01:33:06 GMT  
		Size: 33.2 MB (33188959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc67b41a53412439ff5a0e45f348cfeab80ac0b2fe13df0f07d9873f9207e4c5`  
		Last Modified: Wed, 28 Sep 2022 01:33:04 GMT  
		Size: 8.7 MB (8739499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada940b411031f5a81949b3a09e6a7c7ae44c65367df3b4869c2b2862c499bb9`  
		Last Modified: Wed, 28 Sep 2022 01:33:03 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2db0db4b16adb70c5820ed3af8fa852ee304bc8c56e202b4cb66e0016737d2f`  
		Last Modified: Wed, 28 Sep 2022 01:33:03 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; 386

```console
$ docker pull maven@sha256:d05e1d7bd1be19d7c1185a7cc60303e82f6851fe7fb2cb6964f7f168d8758f48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.6 MB (221628096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0625abafd7a2dd74c16468d1fe031ce43739d44291188293f81e55f22ca097ac`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 06 Sep 2022 18:40:06 GMT
ADD file:31701667cc90b9f4ce7d6ede94bf7dae4d63c49e62d3725094d547f9601e1165 in / 
# Tue, 06 Sep 2022 18:40:07 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 18:56:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 06 Sep 2022 18:56:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Sep 2022 00:58:08 GMT
ENV JAVA_VERSION=8.0.7.16
# Wed, 28 Sep 2022 01:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bb34f647a77ae43611dab3a447da447686352da5426baaff26c22a465dfe40c0';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='b8c35301b56fde151b14e1bfb1374f579f5a0ed361d6ebc7ffff5f82eb563344';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='79fde4473b2c489278fdef105bf69097f1f1a0d54d75a59d24008773b512339b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f1989ee7f41d8d697e880dea74f94133841c2f59ded5c9dd551a26b87f4d36cf';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='eb1cd5b6bf532f10558e7067768d14884d9fce375d2782f91b2218365152bc42';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 28 Sep 2022 01:00:54 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 28 Sep 2022 01:22:38 GMT
RUN apt-get update && apt-get install -y curl
# Wed, 28 Sep 2022 01:22:38 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 28 Sep 2022 01:22:39 GMT
ARG USER_HOME_DIR=/root
# Wed, 28 Sep 2022 01:22:40 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 28 Sep 2022 01:22:41 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 28 Sep 2022 01:22:49 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 28 Sep 2022 01:22:49 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 28 Sep 2022 01:22:50 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 28 Sep 2022 01:22:52 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 28 Sep 2022 01:22:53 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 28 Sep 2022 01:22:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 28 Sep 2022 01:22:54 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:10d3032d1995d3163c20a7f2f197299fae258c2ad020a8fd586fd6b7dd1b0e1d`  
		Last Modified: Tue, 06 Sep 2022 18:40:53 GMT  
		Size: 27.2 MB (27164710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246b95ff97894a60bd98bbfe32df134abb0711c29aae72dd2607024590e794e8`  
		Last Modified: Tue, 06 Sep 2022 18:59:51 GMT  
		Size: 3.0 MB (2983211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66c0e79a445fc4f84ed05644012207e3ad9a0a58870903bc1ebe0b3eb9d02c5`  
		Last Modified: Wed, 28 Sep 2022 01:02:21 GMT  
		Size: 154.5 MB (154504045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb680d6465771c22cc925a2820b475aae58ad595084a7769ec12567952cff7`  
		Last Modified: Wed, 28 Sep 2022 01:23:23 GMT  
		Size: 28.2 MB (28235454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f360e58301150d2019dea99db84714f87d97788d283a68bd6d5cde4fff6e90a`  
		Last Modified: Wed, 28 Sep 2022 01:23:22 GMT  
		Size: 8.7 MB (8739464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b77604fd6db33aa0d02b5ae2ff272abbd8d397890bd95e37d8c103515aad07d`  
		Last Modified: Wed, 28 Sep 2022 01:23:21 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a833be474080bbcd2294b8f17c6af0b05bb1eb5021e88ae8cefc8cd6efafc108`  
		Last Modified: Wed, 28 Sep 2022 01:23:21 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; ppc64le

```console
$ docker pull maven@sha256:0a53de91de73ef02a0b46d42b791ffc70c3f22e9eaf79ef676383c63e9aac0e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.9 MB (233885308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5450a5de525fcfcea1a4ded030964aaf131cab459255456e61e79c204ddecfaa`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:20:27 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 06 Sep 2022 20:20:38 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:20:38 GMT
ENV JAVA_VERSION=8.0.7.15
# Tue, 06 Sep 2022 20:28:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='f042fd06b9312001c7e19cf28194273f25cb5d2b2df4d864b1adfeffa3c8ae7d';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='cb3348717194f19dc08b38021aff2cdbda3e6911e8bcd8e953e909fa212922e4';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='bee2e9e20657f22931e94981822af760c1a7d733134d2cb5dbc6b95bafac8f84';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='6731949f0d61182bc722ee23ba4b2784956afe65ff2ef26ea2e2e125bbff1ef7';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='496b90cdd5ebc279c8e3dbc1acc7c2c0fd8b4ca579ca4b10bbe9a6047b5009cb';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 06 Sep 2022 20:28:32 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Tue, 06 Sep 2022 21:35:50 GMT
RUN apt-get update && apt-get install -y curl
# Tue, 06 Sep 2022 21:35:50 GMT
ARG MAVEN_VERSION=3.8.6
# Tue, 06 Sep 2022 21:35:51 GMT
ARG USER_HOME_DIR=/root
# Tue, 06 Sep 2022 21:35:51 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Tue, 06 Sep 2022 21:35:51 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Tue, 06 Sep 2022 21:35:53 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 06 Sep 2022 21:35:54 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 06 Sep 2022 21:35:54 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 06 Sep 2022 21:35:54 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 06 Sep 2022 21:35:55 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 06 Sep 2022 21:35:55 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 06 Sep 2022 21:35:56 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c293fce30924c9fe30d533e1b557627ce0453d0c3d2f3d7369e05d44a94eb7`  
		Last Modified: Tue, 06 Sep 2022 20:29:05 GMT  
		Size: 3.1 MB (3076075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca21b35ce07e2b858b11f89451c330fe2f52ca056867a0e08f250142b80264f6`  
		Last Modified: Tue, 06 Sep 2022 20:30:22 GMT  
		Size: 166.2 MB (166164093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30d12040f225ff095dbc26457389121a72e1114b64b6402f01d57fc296ec5ee`  
		Last Modified: Tue, 06 Sep 2022 21:38:06 GMT  
		Size: 25.5 MB (25462814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc1a010ae71ce0ef811ecfbb35b7792f8c46fbd50c04c97c5118185ebb430db`  
		Last Modified: Tue, 06 Sep 2022 21:38:03 GMT  
		Size: 8.7 MB (8739496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18ef57155d40364c744b5ef9809539b881613d7bbf4b16773de7740b2159503`  
		Last Modified: Tue, 06 Sep 2022 21:38:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a442ad3fabb0484d7573e573a2b449bf07c983140a44db02c6fdf39d3e65f87`  
		Last Modified: Tue, 06 Sep 2022 21:38:02 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:ibmjava` - linux; s390x

```console
$ docker pull maven@sha256:4ed5dfa4889c19bb8277c9e1d6363f9e2c9bcd49f1622fbd20fe288200f85247
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.1 MB (217070839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aea1d4894609f4b914d328224cf21a9890d67f3f1a7de1a09c141585cb95b1c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 06 Sep 2022 18:43:36 GMT
ADD file:dbe2a8e3943129e654ee29c636cab2bb10dd7eb0ac27d51e6954af2ccbe22807 in / 
# Tue, 06 Sep 2022 18:43:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:00:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 06 Sep 2022 19:00:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Sep 2022 00:52:06 GMT
ENV JAVA_VERSION=8.0.7.16
# Wed, 28 Sep 2022 00:54:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bb34f647a77ae43611dab3a447da447686352da5426baaff26c22a465dfe40c0';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='b8c35301b56fde151b14e1bfb1374f579f5a0ed361d6ebc7ffff5f82eb563344';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='79fde4473b2c489278fdef105bf69097f1f1a0d54d75a59d24008773b512339b';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f1989ee7f41d8d697e880dea74f94133841c2f59ded5c9dd551a26b87f4d36cf';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='eb1cd5b6bf532f10558e7067768d14884d9fce375d2782f91b2218365152bc42';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 28 Sep 2022 00:54:57 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 28 Sep 2022 01:25:47 GMT
RUN apt-get update && apt-get install -y curl
# Wed, 28 Sep 2022 01:25:48 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 28 Sep 2022 01:25:48 GMT
ARG USER_HOME_DIR=/root
# Wed, 28 Sep 2022 01:25:48 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 28 Sep 2022 01:25:48 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 28 Sep 2022 01:25:59 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 28 Sep 2022 01:25:59 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 28 Sep 2022 01:25:59 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 28 Sep 2022 01:25:59 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 28 Sep 2022 01:25:59 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 28 Sep 2022 01:25:59 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 28 Sep 2022 01:26:00 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:be6761156800c616810cb8aeb5b3ae71b9a2082f1c1221210befe119f082e879`  
		Last Modified: Tue, 06 Sep 2022 18:45:00 GMT  
		Size: 25.4 MB (25370130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85df87bfee2629b9bcbd6e19094a6bef3a7109cc473de2f41ee8e4f7d454d2b3`  
		Last Modified: Tue, 06 Sep 2022 19:04:07 GMT  
		Size: 2.7 MB (2671671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0422fb96414156d7c8de730d24dc35ca9626ef215976499145f5450ea1cc7f7b`  
		Last Modified: Wed, 28 Sep 2022 00:56:03 GMT  
		Size: 156.8 MB (156768719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6725daa55cbadc19bfbb9e6f01575627ff0421ba575a4e12f78c27bd143f4df`  
		Last Modified: Wed, 28 Sep 2022 01:27:58 GMT  
		Size: 23.5 MB (23519616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384272dec6d89b536d0d808e6847feef0e91cd32b2436619c2437fdb85e46404`  
		Last Modified: Wed, 28 Sep 2022 01:27:57 GMT  
		Size: 8.7 MB (8739491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30b7f7a18073328c936210820dbda6a014bd0fb132b0595d5220da499e2e0b4`  
		Last Modified: Wed, 28 Sep 2022 01:27:56 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22726e92bec70f7b32ecca06a9a71b559385c8691531eec6209859dbc0fea857`  
		Last Modified: Wed, 28 Sep 2022 01:27:56 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
