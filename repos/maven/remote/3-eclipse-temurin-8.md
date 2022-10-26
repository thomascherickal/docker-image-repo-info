## `maven:3-eclipse-temurin-8`

```console
$ docker pull maven@sha256:82df5b9782987504c023d2bcc152a9ea55c43ac98f0339ca79a0457a76b0a97c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `maven:3-eclipse-temurin-8` - linux; amd64

```console
$ docker pull maven@sha256:55f472e7fe3ecde8b8f056dfe1a38f0f4182e8d9c848780236312e3cfabb36b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176952055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f42c50564b9ea4c998e6d745ed3b1290286ff7dff89cdb5803f1a179cb20a976`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:59:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 16:59:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:59:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 17:00:37 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:00:38 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Wed, 05 Oct 2022 17:00:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='c1965fb24dded7d7944e2da36cd902adf3b7b1d327aaa21ea507cff00a5a0090';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='af4ecd311df32b405142d5756f966418d0200fbf6cb9009c20a44dc691e8da6f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f2be72678f6c2ad283453d0e21a6cb03144dda356e4edf79f818d99c37feaf34';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ed6c9db3719895584fb1fd69fc79c29240977675f26631911c5a1dbce07b7d58';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 05 Oct 2022 17:00:44 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Thu, 06 Oct 2022 03:03:20 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 03:03:21 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 06 Oct 2022 03:03:21 GMT
ARG USER_HOME_DIR=/root
# Thu, 06 Oct 2022 03:03:21 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 06 Oct 2022 03:03:21 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 06 Oct 2022 03:03:24 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 06 Oct 2022 03:03:24 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 06 Oct 2022 03:03:24 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 06 Oct 2022 03:03:24 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 06 Oct 2022 03:03:24 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 06 Oct 2022 03:03:24 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 06 Oct 2022 03:03:24 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7f172af2471a1945e9feb3dab4254026b8c38f20c75ae781436a4495e6db`  
		Last Modified: Wed, 05 Oct 2022 17:07:10 GMT  
		Size: 12.4 MB (12442343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bb7e3e8c3e2df0794920ee96f32424648dea897d3c64b9af15ced4c94978ea`  
		Last Modified: Wed, 05 Oct 2022 17:07:17 GMT  
		Size: 103.5 MB (103515827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4644ab39eedf31f62aa81b7ec8b08413c9119d45150c12784fc23a22694960`  
		Last Modified: Wed, 05 Oct 2022 17:07:08 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00df52191f1714ac7ca0e6d21b485891554e4352d0ffb911fbd52c409d594ae`  
		Last Modified: Thu, 06 Oct 2022 03:09:35 GMT  
		Size: 21.8 MB (21824081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef6838b6c8f4981082fd2744bf037fe6879bd6bde2fcffe103662948121ffac`  
		Last Modified: Thu, 06 Oct 2022 03:09:32 GMT  
		Size: 8.7 MB (8739505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f38e42bba53e4344af8326b1f884965a4a97624854726d72b6a752812a6949`  
		Last Modified: Thu, 06 Oct 2022 03:09:31 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9be09b3577b6a3badfcada612b1a5a9344fff4c9ee40f59e40a0ab45ef096a9`  
		Last Modified: Thu, 06 Oct 2022 03:09:31 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-8` - linux; arm variant v7

```console
$ docker pull maven@sha256:2ecec57a34d521559dc71c112dbc842b4c1ad32cc6428f2e053c7ab5c6619e42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172318136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a172849f3caf8af87a7324d7419dee90f9b5ae1e2c992515089e1f19cabd4f8`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:57 GMT
ADD file:11e25fc4812528219464289700bb0495bf9298918899103c33d7ef9022690eb0 in / 
# Wed, 05 Oct 2022 00:13:57 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:30:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 06 Oct 2022 06:30:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 06:30:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 06 Oct 2022 06:30:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:30:53 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 06 Oct 2022 06:31:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='c1965fb24dded7d7944e2da36cd902adf3b7b1d327aaa21ea507cff00a5a0090';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='af4ecd311df32b405142d5756f966418d0200fbf6cb9009c20a44dc691e8da6f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f2be72678f6c2ad283453d0e21a6cb03144dda356e4edf79f818d99c37feaf34';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ed6c9db3719895584fb1fd69fc79c29240977675f26631911c5a1dbce07b7d58';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 06 Oct 2022 06:31:07 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Fri, 07 Oct 2022 05:57:57 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Oct 2022 05:57:58 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 07 Oct 2022 05:57:58 GMT
ARG USER_HOME_DIR=/root
# Fri, 07 Oct 2022 05:57:58 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 07 Oct 2022 05:57:58 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 07 Oct 2022 05:58:00 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 07 Oct 2022 05:58:00 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 07 Oct 2022 05:58:01 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 07 Oct 2022 05:58:01 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 07 Oct 2022 05:58:01 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 07 Oct 2022 05:58:01 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 07 Oct 2022 05:58:01 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:99b9c73338a7c0dbe41f9fc543fae706650a616453e1e330f870e20916c18a11`  
		Last Modified: Wed, 05 Oct 2022 00:16:02 GMT  
		Size: 27.0 MB (27018632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719b6638b27c56e64e5456f9e5ccd262ec6c6ed045d97ce1df9a938b8e0e1822`  
		Last Modified: Thu, 06 Oct 2022 06:39:41 GMT  
		Size: 12.0 MB (12015320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed177c641227fb789c53678a76a9a1e438dee46c54c14a1b983efd38242e24be`  
		Last Modified: Thu, 06 Oct 2022 06:39:48 GMT  
		Size: 99.2 MB (99176077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bfdad9baa4316ffaa6bdb58153f1736d85b95080e57c7a3887ec88872edd2d`  
		Last Modified: Thu, 06 Oct 2022 06:39:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0c3410778c5e1ec91fc716567940359f8d293e070b8734b32473b90390200c`  
		Last Modified: Fri, 07 Oct 2022 06:03:05 GMT  
		Size: 25.4 MB (25367233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb26545c3eb1ad496f9ec660f8b214e0f1e91529411683c048662098a48bf8c`  
		Last Modified: Fri, 07 Oct 2022 06:03:00 GMT  
		Size: 8.7 MB (8739504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997debb8ad3a18f249e5239b0b3bf98b3aa5e78f02fb9882b3545a2771baae93`  
		Last Modified: Fri, 07 Oct 2022 06:02:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9835cd30a9f8ea018dd3f9121975f15e1f82a41e5b7b92fa673c7f86593c0603`  
		Last Modified: Fri, 07 Oct 2022 06:02:58 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:0807db26fdd8c4badb925e4670bb26f0b8deccd60d9390f72c4a9ba6ad9c0090
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.9 MB (173876232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ad4e279d0d65772cb3ef2a8a9a29e79d2a8b8d49c92954c33ac32b2860742dc`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:02 GMT
ADD file:515177312f20fb1814b89bfccfe695fa2354bbb6d43fdb6e018bf5b1acc17e9f in / 
# Tue, 25 Oct 2022 05:55:02 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:08:29 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 01:08:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 01:08:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 26 Oct 2022 01:09:02 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:09:02 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Wed, 26 Oct 2022 01:09:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='c1965fb24dded7d7944e2da36cd902adf3b7b1d327aaa21ea507cff00a5a0090';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='af4ecd311df32b405142d5756f966418d0200fbf6cb9009c20a44dc691e8da6f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f2be72678f6c2ad283453d0e21a6cb03144dda356e4edf79f818d99c37feaf34';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ed6c9db3719895584fb1fd69fc79c29240977675f26631911c5a1dbce07b7d58';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Oct 2022 01:09:08 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Wed, 26 Oct 2022 15:19:00 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 15:19:00 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 26 Oct 2022 15:19:00 GMT
ARG USER_HOME_DIR=/root
# Wed, 26 Oct 2022 15:19:00 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 26 Oct 2022 15:19:01 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 26 Oct 2022 15:19:08 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 26 Oct 2022 15:19:08 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 26 Oct 2022 15:19:08 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 26 Oct 2022 15:19:08 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 26 Oct 2022 15:19:08 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 26 Oct 2022 15:19:09 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 26 Oct 2022 15:19:09 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:56a2caa6b2c66e01954c1a013b37ea359b6e6af8989dbfb958124b6318771af4`  
		Last Modified: Tue, 25 Oct 2022 05:56:14 GMT  
		Size: 28.4 MB (28382489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d33b973dbba18a894c3b9064cedfece84e92985bce6e3be86a5efef3afdea8`  
		Last Modified: Wed, 26 Oct 2022 01:16:34 GMT  
		Size: 12.4 MB (12400371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1450eb44b38081331cb5a62349c603b45d6d09d6d3c44aa7a6dbf1d8d0f93691`  
		Last Modified: Wed, 26 Oct 2022 01:16:40 GMT  
		Size: 102.6 MB (102615195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33429867dba4a125aa72267ecd6c28be29d991b925a2143e4079348193bbf8e`  
		Last Modified: Wed, 26 Oct 2022 01:16:32 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804a7573cfc0ac5f6bbe0df9ef25037998f61baf733cdbbc57f41b0f04ecad4b`  
		Last Modified: Wed, 26 Oct 2022 15:24:40 GMT  
		Size: 21.7 MB (21737308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27acd2ae323108b9a45a6ca8c5ef1c104c2edadf8c7ba96da34372702dfef4f0`  
		Last Modified: Wed, 26 Oct 2022 15:24:38 GMT  
		Size: 8.7 MB (8739496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced4ad1dd0e71bb36d248d388c8740c31e7647e42640a9b192d01fa2d99a2b47`  
		Last Modified: Wed, 26 Oct 2022 15:24:37 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ced2b43850182dfb11929c175b5568abb0a7e31c05e5725d178c8412388201`  
		Last Modified: Wed, 26 Oct 2022 15:24:37 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-8` - linux; ppc64le

```console
$ docker pull maven@sha256:1c72b0803ca6c6f03582a93b1542f1f25998bd91f83cebacbddd43766a2ec845
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.4 MB (184394216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d96c1d41a900e2b2b56c24355605828fb18493bd13a843a15c7dd4621455139`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:00 GMT
ADD file:766b7743de4ed1a194fc749b7649d245b0cd545b03cc2c81f16a6c15e91c87e7 in / 
# Tue, 25 Oct 2022 03:26:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 13:47:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 13:47:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 13:47:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 13:47:48 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 13:47:49 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Tue, 25 Oct 2022 13:47:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='c1965fb24dded7d7944e2da36cd902adf3b7b1d327aaa21ea507cff00a5a0090';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='af4ecd311df32b405142d5756f966418d0200fbf6cb9009c20a44dc691e8da6f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f2be72678f6c2ad283453d0e21a6cb03144dda356e4edf79f818d99c37feaf34';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ed6c9db3719895584fb1fd69fc79c29240977675f26631911c5a1dbce07b7d58';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 25 Oct 2022 13:48:03 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Wed, 26 Oct 2022 01:23:53 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:23:55 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 26 Oct 2022 01:23:55 GMT
ARG USER_HOME_DIR=/root
# Wed, 26 Oct 2022 01:23:55 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 26 Oct 2022 01:23:55 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 26 Oct 2022 01:23:57 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 26 Oct 2022 01:23:58 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 26 Oct 2022 01:23:58 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 26 Oct 2022 01:23:59 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 26 Oct 2022 01:23:59 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 26 Oct 2022 01:23:59 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 26 Oct 2022 01:24:00 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:aa33126e789290559dc146af02cbf168119ed23be1e30fd99fe8572956e50616`  
		Last Modified: Tue, 25 Oct 2022 03:28:08 GMT  
		Size: 35.7 MB (35709401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222b03548b709077a95a1d389c380123c26cac903f8c75f9ad589c4adad13fe9`  
		Last Modified: Tue, 25 Oct 2022 13:58:58 GMT  
		Size: 13.3 MB (13266255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a1ed6873a605aadf6e3baa13cfdb25eb58df679c98db1d88fddc7f3bcf591`  
		Last Modified: Tue, 25 Oct 2022 13:59:09 GMT  
		Size: 101.0 MB (101009107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032b35d01e7442331eadcfd9abf733d303c1f01691cf0054176128eb4609b056`  
		Last Modified: Tue, 25 Oct 2022 13:58:55 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c42f789bbf1d31a355493a10a1ab0fbe944dedf05cb56f277c15fd8814c89a`  
		Last Modified: Wed, 26 Oct 2022 01:31:00 GMT  
		Size: 25.7 MB (25668581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493f3678e18654e81ab298b5e2abed7967f7806556a0682ccd7ecc8836099594`  
		Last Modified: Wed, 26 Oct 2022 01:30:54 GMT  
		Size: 8.7 MB (8739501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f419813e22afc3dd643fb349469a0c51eff42ab96cfdfc3549171b410157cc2b`  
		Last Modified: Wed, 26 Oct 2022 01:30:52 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93283811dcf43330e2b23048aa067fb9489e67426ab48e3e191c4151fa8d4e`  
		Last Modified: Wed, 26 Oct 2022 01:30:53 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
