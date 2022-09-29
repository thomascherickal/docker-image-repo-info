## `maven:3-eclipse-temurin-19-focal`

```console
$ docker pull maven@sha256:e0a86b31392cdfe7a0e2e6802c3673cedf592c16ad627e3207487273e212b480
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; ppc64le

### `maven:3-eclipse-temurin-19-focal` - linux; amd64

```console
$ docker pull maven@sha256:f728166ec8aa23094f51f590d6ce16176d6333b9d2524781727204af0b2c85c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.5 MB (289457598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d99cab542291f1f110f3679a8db52cdb0a2d48d0c6c431362eb8d4863ec8cd3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:21:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 05:21:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 05:21:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Sep 2022 05:24:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Sep 2022 23:21:02 GMT
ENV JAVA_VERSION=jdk-19+36
# Wed, 28 Sep 2022 17:22:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9b5de40b0f6fe0ab32e8d035720dbbc87bf41b758ed67351ad781ca6505f5294';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jdk_aarch64_linux_hotspot_19_36.tar.gz';          ;;        armhf|arm)          ESUM='34a786548033391de80b857fe02a9c7bd42fcb94243e7273e89012df73f1adef';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jdk_arm_linux_hotspot_19_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='55cc9382227433fa7cc1486a12af59d5bcbea9c40eaeae9608278e056b7d86db';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jdk_ppc64le_linux_hotspot_19_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='d10becfc1ea6586180246455ee8d462875f97655416a7d7c5a1c60d0570dbc8f';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jdk_x64_linux_hotspot_19_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 28 Sep 2022 17:22:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 28 Sep 2022 17:22:43 GMT
CMD ["jshell"]
# Thu, 29 Sep 2022 19:27:31 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Thu, 29 Sep 2022 19:27:31 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 29 Sep 2022 19:27:31 GMT
ARG USER_HOME_DIR=/root
# Thu, 29 Sep 2022 19:27:31 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 29 Sep 2022 19:27:31 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 29 Sep 2022 19:27:33 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 29 Sep 2022 19:27:33 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 29 Sep 2022 19:27:33 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 29 Sep 2022 19:27:33 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 29 Sep 2022 19:27:33 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 29 Sep 2022 19:27:34 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 29 Sep 2022 19:27:34 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b5511391049b7fe5160b78ebae36e40eef43734a07d246dc389dff107a1d22`  
		Last Modified: Fri, 02 Sep 2022 05:30:57 GMT  
		Size: 20.1 MB (20104278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b3a11b0806d9e20a48bdf72b7eb1268cb8edbf32ba42079b7bc91b3a35cddb`  
		Last Modified: Wed, 28 Sep 2022 17:26:03 GMT  
		Size: 200.9 MB (200852810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed96e03b43869418110ca54ae30cafa6fb17192118e5ae6c8f6d11747e8bda16`  
		Last Modified: Wed, 28 Sep 2022 17:25:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2735fdfe9f9f2eb1d2511cc36d4e974bab656b556a27c63e8aeffa7e7a89c5e0`  
		Last Modified: Thu, 29 Sep 2022 19:30:38 GMT  
		Size: 31.2 MB (31186931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c3f355695a1e7066dd510ff84db2c23bd71b747a4ae55bec341c6ca348777d`  
		Last Modified: Thu, 29 Sep 2022 19:30:33 GMT  
		Size: 8.7 MB (8739508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be9bff1485affbe189b826b64ae2513329cc65a5f00e7cce8bf23f088359cbc`  
		Last Modified: Thu, 29 Sep 2022 19:30:33 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3048eb58095b085842671efef05ae9b67c46ece85c3b1ae9e32ae44f945ce39`  
		Last Modified: Thu, 29 Sep 2022 19:30:32 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-19-focal` - linux; ppc64le

```console
$ docker pull maven@sha256:ce6ff00f7b5ca1d0cad8d5d65a5fed4339349f7b4b0c96aa331154f283f21020
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.5 MB (302474925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee9f16a27951dcc6e5b17b808918f33fd67527f840c36d7e2bc61659b8240eb`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 04:00:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 04:00:55 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Sep 2022 04:05:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Sep 2022 17:18:11 GMT
ENV JAVA_VERSION=jdk-19+36
# Wed, 28 Sep 2022 17:18:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9b5de40b0f6fe0ab32e8d035720dbbc87bf41b758ed67351ad781ca6505f5294';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jdk_aarch64_linux_hotspot_19_36.tar.gz';          ;;        armhf|arm)          ESUM='34a786548033391de80b857fe02a9c7bd42fcb94243e7273e89012df73f1adef';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jdk_arm_linux_hotspot_19_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='55cc9382227433fa7cc1486a12af59d5bcbea9c40eaeae9608278e056b7d86db';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jdk_ppc64le_linux_hotspot_19_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='d10becfc1ea6586180246455ee8d462875f97655416a7d7c5a1c60d0570dbc8f';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jdk_x64_linux_hotspot_19_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 28 Sep 2022 17:18:41 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 28 Sep 2022 17:18:42 GMT
CMD ["jshell"]
# Thu, 29 Sep 2022 19:37:11 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Thu, 29 Sep 2022 19:37:12 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 29 Sep 2022 19:37:13 GMT
ARG USER_HOME_DIR=/root
# Thu, 29 Sep 2022 19:37:13 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 29 Sep 2022 19:37:13 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 29 Sep 2022 19:37:15 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 29 Sep 2022 19:37:16 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 29 Sep 2022 19:37:16 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 29 Sep 2022 19:37:17 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 29 Sep 2022 19:37:17 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 29 Sep 2022 19:37:17 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 29 Sep 2022 19:37:18 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be295fe80776586a1665f42f6aa8a3d7eb91486194e2537a9c4651eefea0b183`  
		Last Modified: Fri, 02 Sep 2022 04:16:22 GMT  
		Size: 22.1 MB (22078715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663aa01088f45319d58c243170809cf3e7ad028aa0979c701ba55684de112162`  
		Last Modified: Wed, 28 Sep 2022 17:24:21 GMT  
		Size: 200.0 MB (199965035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6616cfe789c8c76632f0948b866b06728ed8b57168e0bbb78406be3a1c52acd6`  
		Last Modified: Wed, 28 Sep 2022 17:23:48 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3bf34d557a8fea45f25d768e497e4027804cb8543a7cf3fe73e830ff2d8f70`  
		Last Modified: Thu, 29 Sep 2022 19:40:12 GMT  
		Size: 38.4 MB (38394663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1990d22c31373a49ce7399c706c67532eb89c431df985b2b279605330f91b79c`  
		Last Modified: Thu, 29 Sep 2022 19:40:02 GMT  
		Size: 8.7 MB (8739503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdff9c01abe79676ba6b12c7ee93c6274b639b54b3126bc13a4f7588fd2e8397`  
		Last Modified: Thu, 29 Sep 2022 19:40:02 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920df7ca032ea5b59e07418217af78f0b32d5941652f50a985e784457ca8dd2`  
		Last Modified: Thu, 29 Sep 2022 19:40:01 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
