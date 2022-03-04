## `maven:3-eclipse-temurin-16`

```console
$ docker pull maven@sha256:9914da7a302cea421dc91b5b055a7e0fbd80981b69d96f9c7c24df55b21cea65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-eclipse-temurin-16` - linux; amd64

```console
$ docker pull maven@sha256:21893fbf9ecd1e899d6af0970e3f0e5f15a1a3646c59c0f25915c0ff46d98b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.9 MB (303884954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0447ec5065618f9a2b7e5eac5982129677e2a174e1d475a97c96e8878f9179c4`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:33 GMT
ADD file:8a50ad78a668527e974b05a3dfbfd64760de3cb643ceb8a8805d21f6ceab3389 in / 
# Thu, 03 Mar 2022 20:19:33 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 21:23:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 21:25:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 21:25:05 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Thu, 03 Mar 2022 21:25:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cb77d9d126f97898dfdc8b5fb694d1e0e5d93d13a0a6cb2aeda76f8635384340';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_aarch64_linux_hotspot_16.0.2_7.tar.gz';          ;;        armhf|arm)          ESUM='7721ef81416af8122a28448f3d661eb4bda40a9f78d400e4ecc55b58e627a00c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_arm_linux_hotspot_16.0.2_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='36ebe6c72f2fc19b8b17371f731390e15fa3aab08c28b55b9a8b71d0a578adc9';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_ppc64le_linux_hotspot_16.0.2_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fa3ab64ae26727196323105714ac50589ed2782a4c92a29730f7aa886c15807e';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_s390x_linux_hotspot_16.0.2_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='323d6d7474a359a28eff7ddd0df8e65bd61554a8ed12ef42fd9365349e573c2c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_linux_hotspot_16.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 21:25:21 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 21:25:22 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 03 Mar 2022 21:25:22 GMT
CMD ["jshell"]
# Fri, 04 Mar 2022 02:21:42 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 02:21:42 GMT
ARG MAVEN_VERSION=3.8.4
# Fri, 04 Mar 2022 02:21:42 GMT
ARG USER_HOME_DIR=/root
# Fri, 04 Mar 2022 02:21:42 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Fri, 04 Mar 2022 02:21:42 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Fri, 04 Mar 2022 02:21:43 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 04 Mar 2022 02:21:43 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 04 Mar 2022 02:21:44 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 04 Mar 2022 02:21:44 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 04 Mar 2022 02:21:44 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 04 Mar 2022 02:21:44 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 04 Mar 2022 02:21:44 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:7c3b88808835aa80f1ef7f03083c5ae781d0f44e644537cd72de4ce6c5e62e00`  
		Last Modified: Thu, 03 Mar 2022 20:20:44 GMT  
		Size: 28.6 MB (28565751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead8efdcc90ae14990292c6f83165336d0bdeed825c627da155c6d6acd9fb5ed`  
		Last Modified: Thu, 03 Mar 2022 21:28:53 GMT  
		Size: 28.6 MB (28566161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569c4e2abf81babbf26c92a5e8e679de66af20c96648f6312b8404d86272318e`  
		Last Modified: Thu, 03 Mar 2022 21:29:05 GMT  
		Size: 206.5 MB (206462441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac100709b4c7f0513da9c8eb0f00952e046d954433e8cff1d19efc5c1f7fbfe`  
		Last Modified: Thu, 03 Mar 2022 21:28:47 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cfdb49c884467c4bd8c8311282abf9b176a234ee6aa1b4b64b525f6c4a5072a`  
		Last Modified: Fri, 04 Mar 2022 02:25:38 GMT  
		Size: 31.2 MB (31179431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a4395b562d180b0ac3781d5da8a4d8fc5e4dae4433fcc1ffde6cb4c2353ba4`  
		Last Modified: Fri, 04 Mar 2022 02:25:34 GMT  
		Size: 9.1 MB (9109801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bde9356827bef4ce4209a35d86187ca46e9d206abc9d0b2bc9bc9357db420d`  
		Last Modified: Fri, 04 Mar 2022 02:25:33 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed139877c57222ac20d013dd4d178bdbe8b3ebd52d87ce5b0fd423b18a49ec21`  
		Last Modified: Fri, 04 Mar 2022 02:25:33 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-16` - linux; arm variant v7

```console
$ docker pull maven@sha256:39587a2250881c99a231c1f14f2bec452f434d9c4808f7b15c936ea1265a8860
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.4 MB (276353492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5114945a8ff971d71f1f28be3d4be1aed945420f4aa6e5a65a1d71c37547039d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 02 Feb 2022 02:25:11 GMT
ADD file:0adc3f597b5ba8c31a9a4d67126166cf067749754e269fe2c3ed43f03457b53c in / 
# Wed, 02 Feb 2022 02:25:12 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:47:09 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:50:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:50:12 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Wed, 02 Feb 2022 02:50:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cb77d9d126f97898dfdc8b5fb694d1e0e5d93d13a0a6cb2aeda76f8635384340';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_aarch64_linux_hotspot_16.0.2_7.tar.gz';          ;;        armhf|arm)          ESUM='7721ef81416af8122a28448f3d661eb4bda40a9f78d400e4ecc55b58e627a00c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_arm_linux_hotspot_16.0.2_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='36ebe6c72f2fc19b8b17371f731390e15fa3aab08c28b55b9a8b71d0a578adc9';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_ppc64le_linux_hotspot_16.0.2_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fa3ab64ae26727196323105714ac50589ed2782a4c92a29730f7aa886c15807e';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_s390x_linux_hotspot_16.0.2_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='323d6d7474a359a28eff7ddd0df8e65bd61554a8ed12ef42fd9365349e573c2c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_linux_hotspot_16.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:50:42 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:50:45 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 02 Feb 2022 02:50:45 GMT
CMD ["jshell"]
# Mon, 14 Feb 2022 19:59:31 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Mon, 14 Feb 2022 19:59:32 GMT
ARG MAVEN_VERSION=3.8.4
# Mon, 14 Feb 2022 19:59:33 GMT
ARG USER_HOME_DIR=/root
# Mon, 14 Feb 2022 19:59:33 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Mon, 14 Feb 2022 19:59:34 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Mon, 14 Feb 2022 19:59:43 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 14 Feb 2022 19:59:43 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 14 Feb 2022 19:59:44 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 14 Feb 2022 19:59:44 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 14 Feb 2022 19:59:45 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 14 Feb 2022 19:59:45 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 14 Feb 2022 19:59:46 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:42bcffb5d2901aadaedc35f036cf725a537494a5869ae378ec427d313ff41fa6`  
		Last Modified: Wed, 02 Feb 2022 02:29:41 GMT  
		Size: 24.1 MB (24062751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c0154b8e60d06ef2e654b6fc885e6b2f15bdad4767412580dc35e38d769ec3`  
		Last Modified: Wed, 02 Feb 2022 02:56:28 GMT  
		Size: 27.4 MB (27368116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0a1c1aec4e37da2c2a943c6dc9d3d35a9f8e142718646bfee8e706af553827`  
		Last Modified: Wed, 02 Feb 2022 02:57:22 GMT  
		Size: 188.5 MB (188506873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f12b09e126656d9acdad5940a043f67e734784cb702d0e247183a3894267d3`  
		Last Modified: Wed, 02 Feb 2022 02:56:09 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff08d46f15050c70b452a0079cf379826aa383243462d7001e90076632a5474`  
		Last Modified: Mon, 14 Feb 2022 20:03:55 GMT  
		Size: 27.3 MB (27304573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11815b5c0b3de33bdd48d00ef17cc0866d4aa3a3f5775ed20affd4f955c51393`  
		Last Modified: Mon, 14 Feb 2022 20:03:40 GMT  
		Size: 9.1 MB (9109805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d91a5f1b196e17b20b096de2396ff1ccda65eaf44c16c1b7b3f2ee9f2f651ab`  
		Last Modified: Mon, 14 Feb 2022 20:03:38 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ea44b804c6b1d9e41e2d7013a61332c175b81aec32d16de0251532ae69cb03`  
		Last Modified: Mon, 14 Feb 2022 20:03:38 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-16` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:adc4f00a30e613cec2d8674caa1410dfd3918610fa648dad3c87aa0b3252b959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.8 MB (300760786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8572751d73d06144d52b8597935000557e0f0289483c547d74d128b9f9efec22`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 03 Mar 2022 19:41:02 GMT
ADD file:f2fffe739729839aa17484bc4d79d33425549c5052824eac12131b16c23565d3 in / 
# Thu, 03 Mar 2022 19:41:03 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 20:21:02 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 20:23:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 20:23:10 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Thu, 03 Mar 2022 20:23:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cb77d9d126f97898dfdc8b5fb694d1e0e5d93d13a0a6cb2aeda76f8635384340';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_aarch64_linux_hotspot_16.0.2_7.tar.gz';          ;;        armhf|arm)          ESUM='7721ef81416af8122a28448f3d661eb4bda40a9f78d400e4ecc55b58e627a00c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_arm_linux_hotspot_16.0.2_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='36ebe6c72f2fc19b8b17371f731390e15fa3aab08c28b55b9a8b71d0a578adc9';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_ppc64le_linux_hotspot_16.0.2_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fa3ab64ae26727196323105714ac50589ed2782a4c92a29730f7aa886c15807e';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_s390x_linux_hotspot_16.0.2_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='323d6d7474a359a28eff7ddd0df8e65bd61554a8ed12ef42fd9365349e573c2c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_linux_hotspot_16.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 20:23:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 20:23:25 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 03 Mar 2022 20:23:25 GMT
CMD ["jshell"]
# Thu, 03 Mar 2022 23:20:19 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 23:20:19 GMT
ARG MAVEN_VERSION=3.8.4
# Thu, 03 Mar 2022 23:20:20 GMT
ARG USER_HOME_DIR=/root
# Thu, 03 Mar 2022 23:20:21 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Thu, 03 Mar 2022 23:20:22 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Thu, 03 Mar 2022 23:20:37 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 03 Mar 2022 23:20:38 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 03 Mar 2022 23:20:39 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 03 Mar 2022 23:20:41 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 03 Mar 2022 23:20:42 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 03 Mar 2022 23:20:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 03 Mar 2022 23:20:43 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5a7855fb0d7ae372c824d9c76be5ad2f42ce178c1910fa54a8543036b5325fd5`  
		Last Modified: Thu, 03 Mar 2022 19:42:38 GMT  
		Size: 27.2 MB (27169631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7afec2522dcf8183cf124997a84e381fcddfe101348ae644fdd54a349167ef`  
		Last Modified: Thu, 03 Mar 2022 20:27:34 GMT  
		Size: 29.4 MB (29380102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ee67547cbb6ee6f0e578b29921c0d8ea2f0b0800750af3db31edcff1b50973`  
		Last Modified: Thu, 03 Mar 2022 20:27:51 GMT  
		Size: 204.1 MB (204124263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf15aedb94b70c3d2a733101492f4d2dff8f197261ef7388c962cce61b42a21`  
		Last Modified: Thu, 03 Mar 2022 20:27:29 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfd36b8ef03168e3184ff6af24a6a7fb8f2e77005f6e75b52bec6c691cb43a8`  
		Last Modified: Thu, 03 Mar 2022 23:27:36 GMT  
		Size: 31.0 MB (30975674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0d1643a6dfef4487693d2d171e3cd608c5b581948c81f9dbd945b228130a5d`  
		Last Modified: Thu, 03 Mar 2022 23:27:32 GMT  
		Size: 9.1 MB (9109772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24711e41bb03b0724363020da202601c2139557f55c162bba46039be5f4869eb`  
		Last Modified: Thu, 03 Mar 2022 23:27:31 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b14fbd4dd69706b404b85db4bd75838d9faf5b259d6569eead85344057eb2ea`  
		Last Modified: Thu, 03 Mar 2022 23:27:31 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-16` - linux; ppc64le

```console
$ docker pull maven@sha256:cc6d5eb4500b10feada27e4c493b77e4d15a09f936abd3257a8958a97a039fef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.9 MB (298859339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0068c897791378a5931cacfe86677132282e2021e067f72506c290b972f53a9c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 03 Mar 2022 20:28:30 GMT
ADD file:039f04ac6c5dbbe3fb0a5eee16945cf7c5fb7565751d6bdf8ec0c1102798c1de in / 
# Thu, 03 Mar 2022 20:28:38 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 22:04:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 22:11:42 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:11:47 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Thu, 03 Mar 2022 22:12:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cb77d9d126f97898dfdc8b5fb694d1e0e5d93d13a0a6cb2aeda76f8635384340';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_aarch64_linux_hotspot_16.0.2_7.tar.gz';          ;;        armhf|arm)          ESUM='7721ef81416af8122a28448f3d661eb4bda40a9f78d400e4ecc55b58e627a00c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_arm_linux_hotspot_16.0.2_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='36ebe6c72f2fc19b8b17371f731390e15fa3aab08c28b55b9a8b71d0a578adc9';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_ppc64le_linux_hotspot_16.0.2_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fa3ab64ae26727196323105714ac50589ed2782a4c92a29730f7aa886c15807e';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_s390x_linux_hotspot_16.0.2_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='323d6d7474a359a28eff7ddd0df8e65bd61554a8ed12ef42fd9365349e573c2c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_linux_hotspot_16.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 22:12:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 22:12:31 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 03 Mar 2022 22:12:36 GMT
CMD ["jshell"]
# Fri, 04 Mar 2022 02:02:33 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 02:02:41 GMT
ARG MAVEN_VERSION=3.8.4
# Fri, 04 Mar 2022 02:02:45 GMT
ARG USER_HOME_DIR=/root
# Fri, 04 Mar 2022 02:02:48 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Fri, 04 Mar 2022 02:02:54 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Fri, 04 Mar 2022 02:03:02 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 04 Mar 2022 02:03:05 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 04 Mar 2022 02:03:11 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 04 Mar 2022 02:03:13 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 04 Mar 2022 02:03:15 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 04 Mar 2022 02:03:20 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 04 Mar 2022 02:03:26 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a16b43de69d1e799ea2cb675e7e605db0ff3a8d692fd326fbde80a370e0676d5`  
		Last Modified: Thu, 03 Mar 2022 20:33:55 GMT  
		Size: 33.3 MB (33292195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849817e98afbf9ee5cdf1650e92b780ddfc3ab08fd11774b21e9643406ae1ca9`  
		Last Modified: Thu, 03 Mar 2022 22:18:39 GMT  
		Size: 31.1 MB (31122304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa305cb2693bd8ffc9d3631d2e733478505ff22766504b46d1f6bd505c1dbb1`  
		Last Modified: Thu, 03 Mar 2022 22:18:55 GMT  
		Size: 186.9 MB (186948185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1b9e928e01ca5eaa9704c5c7fe8aa3787dab1fa53da8920e047b78fa64be41`  
		Last Modified: Thu, 03 Mar 2022 22:18:33 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6a9f2c2c197e10a5e3c023b29f2b71121b7211187984be2c5f1d2c866ad2c8`  
		Last Modified: Fri, 04 Mar 2022 02:12:33 GMT  
		Size: 38.4 MB (38385480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae9bf85f8caa201382f6c767a9ede8891771ca840761be42d7703b414311d41`  
		Last Modified: Fri, 04 Mar 2022 02:12:27 GMT  
		Size: 9.1 MB (9109804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0f4368132008c9968122b01e5063d9d753f16ca65a089703490d43d26410c7`  
		Last Modified: Fri, 04 Mar 2022 02:12:26 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62666feb81c77b9ed379e9c22537418625fc878cc82cdf5da907fe396975bf31`  
		Last Modified: Fri, 04 Mar 2022 02:12:26 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-16` - linux; s390x

```console
$ docker pull maven@sha256:45e02c4cb0350380a52d7274e22108cbf78128cd9a15925251cbafefcef3e3cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274675061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe7dd37baca64a3d7e69a144d836e8a5cc3905c764699a62531bb63913cd9f9f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 03 Mar 2022 19:41:52 GMT
ADD file:3162233da685a36a9f274a7fa1d99452cab76f37e3640d38851c782ca506f75b in / 
# Thu, 03 Mar 2022 19:41:53 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 19:59:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 20:00:21 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 20:00:22 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Thu, 03 Mar 2022 20:00:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cb77d9d126f97898dfdc8b5fb694d1e0e5d93d13a0a6cb2aeda76f8635384340';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_aarch64_linux_hotspot_16.0.2_7.tar.gz';          ;;        armhf|arm)          ESUM='7721ef81416af8122a28448f3d661eb4bda40a9f78d400e4ecc55b58e627a00c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_arm_linux_hotspot_16.0.2_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='36ebe6c72f2fc19b8b17371f731390e15fa3aab08c28b55b9a8b71d0a578adc9';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_ppc64le_linux_hotspot_16.0.2_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fa3ab64ae26727196323105714ac50589ed2782a4c92a29730f7aa886c15807e';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_s390x_linux_hotspot_16.0.2_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='323d6d7474a359a28eff7ddd0df8e65bd61554a8ed12ef42fd9365349e573c2c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_linux_hotspot_16.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 20:00:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 20:00:35 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 03 Mar 2022 20:00:35 GMT
CMD ["jshell"]
# Thu, 03 Mar 2022 21:03:47 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 21:03:48 GMT
ARG MAVEN_VERSION=3.8.4
# Thu, 03 Mar 2022 21:03:48 GMT
ARG USER_HOME_DIR=/root
# Thu, 03 Mar 2022 21:03:48 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Thu, 03 Mar 2022 21:03:49 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Thu, 03 Mar 2022 21:03:56 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 03 Mar 2022 21:03:56 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 03 Mar 2022 21:03:56 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 03 Mar 2022 21:03:56 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 03 Mar 2022 21:03:56 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 03 Mar 2022 21:03:56 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 03 Mar 2022 21:03:56 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:ade7e68f4e34f438527a34c9761a285c3c3864e3daab0544b2c4f4163c7c3f56`  
		Last Modified: Thu, 03 Mar 2022 19:43:22 GMT  
		Size: 27.1 MB (27084671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67794419b7271832d65da191bde592a4c2e4dbf8f986cd2cde08544ec953bcfc`  
		Last Modified: Thu, 03 Mar 2022 20:02:48 GMT  
		Size: 27.9 MB (27942763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cc1e758600826c5335ab26e0fe44fb1c584bc8b8c20890a60ce058443df604`  
		Last Modified: Thu, 03 Mar 2022 20:02:56 GMT  
		Size: 179.8 MB (179837114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f9e7b3d94b21e69baa7397d471e8eb37cee40737411559dfd95212bf2d5f9c`  
		Last Modified: Thu, 03 Mar 2022 20:02:45 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5327e60f1e6cb40f3a146355ce52e778b747e460d397e6ef85b650274adcb587`  
		Last Modified: Thu, 03 Mar 2022 21:07:08 GMT  
		Size: 30.7 MB (30699313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d57ee8bc73cc31d3bad602f84125c6b32c5666b3ba137fcc3c38f45f01b082`  
		Last Modified: Thu, 03 Mar 2022 21:07:05 GMT  
		Size: 9.1 MB (9109825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a289f8d6ce77fed0c623ae52594e7f1e1403d127166600e34b51a82cb6741981`  
		Last Modified: Thu, 03 Mar 2022 21:07:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8170e9e42c1934d33c82facd8576f7cceab7769bc50f7d3f57cce77cb598d58`  
		Last Modified: Thu, 03 Mar 2022 21:07:04 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
