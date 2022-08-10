## `maven:3-ibm-semeru-17-focal`

```console
$ docker pull maven@sha256:6a13a8ba44e76dc2d1bbc97806eb6d558d41f4e0af65220c22bf7aa9c9ca90c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-ibm-semeru-17-focal` - linux; amd64

```console
$ docker pull maven@sha256:67d4232cf55f0ec2cd48db275e325089decbdf8b0d7be005a8c0eb13ddcf8131
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.8 MB (298804147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8abf2e6a4962a25f3c0b391aa72a217347a29cb2cbc9a5fef32faab66d010ca8`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 10 Aug 2022 22:48:51 GMT
ENV JAVA_VERSION=jdk-17.0.4+8_openj9-0.33.0
# Wed, 10 Aug 2022 22:49:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='18d291411ee4a956018b4dcefe436971e73694128782617f1b44beca991956c5';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.4%2B8_openj9-0.33.0/ibm-semeru-open-jdk_aarch64_linux_17.0.4_8_openj9-0.33.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78ae15d9e01fce3a473f4d6a90c331fb766211b950931088c2a85590f178ad39';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.4%2B8_openj9-0.33.0/ibm-semeru-open-jdk_x64_linux_17.0.4_8_openj9-0.33.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8f69c221fe25a37d645415819ce01d81dfaef5073d87b237e4108d28486dd5f4';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.4%2B8_openj9-0.33.0/ibm-semeru-open-jdk_ppc64le_linux_17.0.4_8_openj9-0.33.0.tar.gz';          ;;        s390x)          ESUM='af09945bd4bcbd10dbf18d1df2400bfe04b9e76de5fae1b40e37463ba2080641';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.4%2B8_openj9-0.33.0/ibm-semeru-open-jdk_s390x_linux_17.0.4_8_openj9-0.33.0.tar.gz';          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 10 Aug 2022 22:49:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 22:49:20 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 10 Aug 2022 22:49:55 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 10 Aug 2022 22:49:55 GMT
CMD ["jshell"]
# Wed, 10 Aug 2022 23:19:30 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Wed, 10 Aug 2022 23:19:30 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 10 Aug 2022 23:19:31 GMT
ARG USER_HOME_DIR=/root
# Wed, 10 Aug 2022 23:19:31 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 10 Aug 2022 23:19:31 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 10 Aug 2022 23:19:39 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 10 Aug 2022 23:19:39 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 10 Aug 2022 23:19:39 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 10 Aug 2022 23:19:39 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 10 Aug 2022 23:19:39 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 10 Aug 2022 23:19:39 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 10 Aug 2022 23:19:39 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398d776e32fac0ec8c2698a6d7bc5d81c5d35de32a68fb2d7882e0f46b73fd37`  
		Last Modified: Tue, 02 Aug 2022 19:13:20 GMT  
		Size: 16.0 MB (16029939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c239e48d8129b86d2f85b7d93c1154db8629ceaf4da4069b7297b8b8a5ffdd98`  
		Last Modified: Wed, 10 Aug 2022 22:59:54 GMT  
		Size: 208.3 MB (208348310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5536ebd5f76c1ac4dbd7ec86a2c845acb1fbdc3f47e706853589de71231d2f41`  
		Last Modified: Wed, 10 Aug 2022 22:59:40 GMT  
		Size: 5.9 MB (5928798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34de30a0f451a706320d4717f5d51605f12dcc511ac1dd9c488bc004e3069e21`  
		Last Modified: Wed, 10 Aug 2022 23:22:23 GMT  
		Size: 31.2 MB (31183778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a178ae0cf7d555d41089b7b9917b12b7b93d3e69c852cb7698aa443903054`  
		Last Modified: Wed, 10 Aug 2022 23:22:19 GMT  
		Size: 8.7 MB (8739512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9817f2b9a78b734bab0eb97791c83ba4a763c55124baa4523f3e99e6400b4a`  
		Last Modified: Wed, 10 Aug 2022 23:22:18 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18e1d63aa2fab468d7d9d5b2a06fc4ea6405e827ea1d57e8e0f60396aaa7a75`  
		Last Modified: Wed, 10 Aug 2022 23:22:19 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibm-semeru-17-focal` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:5b1111625d1fd4a9fe1e802997820eee6cfb756fc2ecc1029a5e531c27f83739
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.1 MB (292139513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1bd1c31933eb26e514fb47ae7e5ef8339d028110335b7ceba20e581ca46a1e`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:50:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 17:51:12 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:12:44 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 18:13:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='07ee14c56e9f371a18887b907e03ee3f297ef2a535521e9d0624ac0b033dd35f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jdk_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7dca04533d539675cc22d60d567b660bbf9a5a8c6ce832a189caea753590bbdd';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jdk_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='c0b667f735c19f7d4ce0ef594354b46866660b7648727bf7f4b9bea5f9464790';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jdk_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='68ad59228c05674c39ebbd3dc4d8997a21e4c413b5522d0c0e27098dca920895';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jdk_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 18:13:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 18:13:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 18:13:37 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 02 Aug 2022 18:13:38 GMT
CMD ["jshell"]
# Wed, 03 Aug 2022 01:09:04 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 01:09:04 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 03 Aug 2022 01:09:05 GMT
ARG USER_HOME_DIR=/root
# Wed, 03 Aug 2022 01:09:06 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 03 Aug 2022 01:09:07 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 03 Aug 2022 01:09:17 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 03 Aug 2022 01:09:18 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 03 Aug 2022 01:09:19 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 03 Aug 2022 01:09:21 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 03 Aug 2022 01:09:22 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 03 Aug 2022 01:09:22 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 03 Aug 2022 01:09:23 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf715bbfc12ff844d7de72d6ff70e4c89116b7db5bed3c7bc1c776ee4f99a77`  
		Last Modified: Tue, 02 Aug 2022 17:59:38 GMT  
		Size: 15.9 MB (15891207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1071755b4a6d6f8465fbe1c9b312a3ce7efa77e616c8b40646a0bd4f338a88`  
		Last Modified: Tue, 02 Aug 2022 18:20:09 GMT  
		Size: 203.6 MB (203608243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b4b8433c17b2c6d13201b316a463f1b220f49569436556c70e30545b8440f`  
		Last Modified: Tue, 02 Aug 2022 18:19:53 GMT  
		Size: 5.7 MB (5723703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7444578a6ed8aa5435787c93b68beb6a35a5ae9720298f55d02425c0cb746579`  
		Last Modified: Wed, 03 Aug 2022 01:17:16 GMT  
		Size: 31.0 MB (30983869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17eccfaec14895a755432f96b40cdd2752413cb89421347c98bf5319260e14ff`  
		Last Modified: Wed, 03 Aug 2022 01:17:12 GMT  
		Size: 8.7 MB (8739472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a0fcab1ce866234e7c0dca9d484037f110b0ee54f0282249edbe567e03f369`  
		Last Modified: Wed, 03 Aug 2022 01:17:11 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491a2e1ffe358d9f9d057f918f229b35ee1fdc6938fdeb175aabb0f82b5c8c44`  
		Last Modified: Wed, 03 Aug 2022 01:17:11 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibm-semeru-17-focal` - linux; ppc64le

```console
$ docker pull maven@sha256:5081cc56d5d887939b98039e00edc5cda3e0f0cb6590984a2d96c75ee1d547f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.6 MB (311624059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86923edb6d23cab6fb8dbe6341827003424c953fdd72a4f8488b4a80d227e619`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 03:18:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 03 Aug 2022 03:20:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 04:07:48 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Wed, 03 Aug 2022 04:08:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='07ee14c56e9f371a18887b907e03ee3f297ef2a535521e9d0624ac0b033dd35f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jdk_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='7dca04533d539675cc22d60d567b660bbf9a5a8c6ce832a189caea753590bbdd';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jdk_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='c0b667f735c19f7d4ce0ef594354b46866660b7648727bf7f4b9bea5f9464790';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jdk_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='68ad59228c05674c39ebbd3dc4d8997a21e4c413b5522d0c0e27098dca920895';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jdk_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 03 Aug 2022 04:08:14 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 04:08:14 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 03 Aug 2022 04:08:52 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 04:08:52 GMT
CMD ["jshell"]
# Wed, 03 Aug 2022 23:50:32 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 23:50:34 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 03 Aug 2022 23:50:34 GMT
ARG USER_HOME_DIR=/root
# Wed, 03 Aug 2022 23:50:34 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 03 Aug 2022 23:50:34 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 03 Aug 2022 23:50:36 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 03 Aug 2022 23:50:37 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 03 Aug 2022 23:50:37 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 03 Aug 2022 23:50:38 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 03 Aug 2022 23:50:38 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 03 Aug 2022 23:50:38 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 03 Aug 2022 23:50:39 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93d2375ba0032ebd673deba460fc14719ca1d2863b8d267e076565f71f6a0a6`  
		Last Modified: Wed, 03 Aug 2022 03:33:39 GMT  
		Size: 17.2 MB (17202740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236e617efc003fa05c6d77e9dc44b2e9137468348413bfe85c295f9aeb63adb8`  
		Last Modified: Wed, 03 Aug 2022 04:25:20 GMT  
		Size: 209.1 MB (209134442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac36cf5c7bb768bdf3977178c75f125d482f730270494381b05c47b433f26aaf`  
		Last Modified: Wed, 03 Aug 2022 04:24:55 GMT  
		Size: 4.9 MB (4861096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcb04156077060a97b097c6781ee74010b47ee68a4aa7d88142e10628602d26`  
		Last Modified: Wed, 03 Aug 2022 23:56:57 GMT  
		Size: 38.4 MB (38389717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0ab971f11660046ff1727f1f8887a758aea46f7272105bd9199a057f861f97`  
		Last Modified: Wed, 03 Aug 2022 23:56:48 GMT  
		Size: 8.7 MB (8739503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7eb14e9a4b369a8746465b9987714dfb57bd51db19b4da7e3439bb458fd95e`  
		Last Modified: Wed, 03 Aug 2022 23:56:47 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e9b9f70395a8547733887bc72731aa8f2e489f1adfa5905b2b3698b2bcbd55`  
		Last Modified: Wed, 03 Aug 2022 23:56:47 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibm-semeru-17-focal` - linux; s390x

```console
$ docker pull maven@sha256:3b128ca3648a9473378256e483115e1edfa46ef4e284c71a04f606661b89b69b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294524468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8573be4e8e0d6c6daeafd5f05a185877bb94d390ff37a10d907d2256ea1bf942`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 10 Aug 2022 21:46:23 GMT
ENV JAVA_VERSION=jdk-17.0.4+8_openj9-0.33.0
# Wed, 10 Aug 2022 21:46:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='18d291411ee4a956018b4dcefe436971e73694128782617f1b44beca991956c5';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.4%2B8_openj9-0.33.0/ibm-semeru-open-jdk_aarch64_linux_17.0.4_8_openj9-0.33.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78ae15d9e01fce3a473f4d6a90c331fb766211b950931088c2a85590f178ad39';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.4%2B8_openj9-0.33.0/ibm-semeru-open-jdk_x64_linux_17.0.4_8_openj9-0.33.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8f69c221fe25a37d645415819ce01d81dfaef5073d87b237e4108d28486dd5f4';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.4%2B8_openj9-0.33.0/ibm-semeru-open-jdk_ppc64le_linux_17.0.4_8_openj9-0.33.0.tar.gz';          ;;        s390x)          ESUM='af09945bd4bcbd10dbf18d1df2400bfe04b9e76de5fae1b40e37463ba2080641';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.4%2B8_openj9-0.33.0/ibm-semeru-open-jdk_s390x_linux_17.0.4_8_openj9-0.33.0.tar.gz';          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 10 Aug 2022 21:46:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 21:46:47 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 10 Aug 2022 21:47:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 10 Aug 2022 21:47:26 GMT
CMD ["jshell"]
# Wed, 10 Aug 2022 22:25:13 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Wed, 10 Aug 2022 22:25:15 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 10 Aug 2022 22:25:15 GMT
ARG USER_HOME_DIR=/root
# Wed, 10 Aug 2022 22:25:15 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 10 Aug 2022 22:25:15 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 10 Aug 2022 22:25:30 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 10 Aug 2022 22:25:30 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 10 Aug 2022 22:25:30 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 10 Aug 2022 22:25:31 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 10 Aug 2022 22:25:31 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 10 Aug 2022 22:25:31 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 10 Aug 2022 22:25:31 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d522b75fb69271e75617d2e7bbeede1210f48bffdc57121ee39534eea94e2815`  
		Last Modified: Tue, 02 Aug 2022 01:03:38 GMT  
		Size: 27.0 MB (27045363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204f6f9c0aa5d9c3e1300660817d3dd41177073448243d9ccc18a39c3f14083a`  
		Last Modified: Tue, 02 Aug 2022 12:52:19 GMT  
		Size: 15.7 MB (15730128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd92274b2cda485c9253aff54f9dfa86c3c53ccb443d00121c0320404a4de652`  
		Last Modified: Wed, 10 Aug 2022 21:58:36 GMT  
		Size: 206.3 MB (206278798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabea178a17503cb1751b5a61b14155d10582d616b5f79c7389b0ed216a72c01`  
		Last Modified: Wed, 10 Aug 2022 21:58:27 GMT  
		Size: 6.0 MB (6034520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3414d1741b32b50bc5cf9565b2c7b9230796438655b361e3d9fa7cc1502dcd1`  
		Last Modified: Wed, 10 Aug 2022 22:29:44 GMT  
		Size: 30.7 MB (30694964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a321df7da45770ed9e858919027bba9c02d373f14ff811f29e5281461f4968b4`  
		Last Modified: Wed, 10 Aug 2022 22:29:44 GMT  
		Size: 8.7 MB (8739481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf798e04c264b32920bf41142218c8eac5416dc95327e22ded9a353bc02b1e0`  
		Last Modified: Wed, 10 Aug 2022 22:29:44 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79fe36e76d636b03d6994199687702acfa25661f2921b2baa17a5cc1f1124aa`  
		Last Modified: Wed, 10 Aug 2022 22:29:44 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
