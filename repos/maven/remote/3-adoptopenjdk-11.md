## `maven:3-adoptopenjdk-11`

```console
$ docker pull maven@sha256:ce304bcbf3a4d0190ed0ee1eb4dabdcc68ee70cd04bf3616c662dfb497c125c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-adoptopenjdk-11` - linux; amd64

```console
$ docker pull maven@sha256:ce03b36ee711f241b54c85a63f7a321d98ad7ebb483d84c1992662d7c328800c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.8 MB (278829018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5534cbdebdbe881e23f985d6c42798c408922272fba3c080c559674e882ebf90`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:59:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 26 Jul 2021 22:59:58 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:00:18 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Mon, 26 Jul 2021 23:00:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4966b0df9406b7041e14316e04c9579806832fafa02c5d3bd1842163b7f2353a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.11_9.tar.gz';          ;;        armhf|armv7l)          ESUM='2d7aba0b9ea287145ad437d4b3035fc84f7508e78c6fec99be4ff59fe1b6fc0d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.11_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='945b114bd0a617d742653ac1ae89d35384bf89389046a44681109cf8e4f4af91';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.11_9.tar.gz';          ;;        s390x)          ESUM='5d81979d27d9d8b3ed5bca1a91fc899cbbfb3d907f445ee7329628105e92f52c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.11_9.tar.gz';          ;;        amd64|x86_64)          ESUM='e99b98f851541202ab64401594901e583b764e368814320eba442095251e78cb';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.11_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 26 Jul 2021 23:00:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 26 Jul 2021 23:00:28 GMT
CMD ["jshell"]
# Mon, 16 Aug 2021 17:26:39 GMT
ARG MAVEN_VERSION=3.8.2
# Mon, 16 Aug 2021 17:26:39 GMT
ARG USER_HOME_DIR=/root
# Mon, 16 Aug 2021 17:26:39 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Mon, 16 Aug 2021 17:26:39 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Mon, 16 Aug 2021 17:27:03 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:27:09 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 16 Aug 2021 17:27:09 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 16 Aug 2021 17:27:10 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 16 Aug 2021 17:27:10 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 16 Aug 2021 17:27:10 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 16 Aug 2021 17:27:10 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 16 Aug 2021 17:27:10 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f63509f5b973d2357463075b878f6ff9177d80ba67e8544cc72eaf22ae30959`  
		Last Modified: Mon, 26 Jul 2021 23:09:43 GMT  
		Size: 16.0 MB (16033263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d7b43f221b36cd41283789af5d5c79d64a5a47c627fa8295a0f307a00aa861`  
		Last Modified: Mon, 26 Jul 2021 23:10:34 GMT  
		Size: 193.7 MB (193651025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23166023410413c5cb7681bac17a09dcc3f1033de35cb1736dd87e1b6349b98`  
		Last Modified: Mon, 16 Aug 2021 17:36:51 GMT  
		Size: 31.2 MB (31170111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f137399ccc9de78fbbe7f9c848a7f1cc260bc1e58742eeb70dccbf361be331b`  
		Last Modified: Mon, 16 Aug 2021 17:36:46 GMT  
		Size: 9.4 MB (9405462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d79d8d60985cb3519f59bdc6132178a4ffd1fa33d002d51d419ab213a38a712`  
		Last Modified: Mon, 16 Aug 2021 17:36:46 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d899d79d2f1fcc7ff46400ee520387d5122c085b2af7c7438c9b01dc812da189`  
		Last Modified: Mon, 16 Aug 2021 17:36:46 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk-11` - linux; arm variant v7

```console
$ docker pull maven@sha256:916627c5437fc330a88ea5b2d1de2c5ca20f02577f7f211849a08f4d8f7adbdf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.4 MB (257416820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d14f4fa17b021d1fab1f0ed45eac1c29b21f3a1a5c9297bc0bb37bedebe93c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:51:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 02:52:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:53:03 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Tue, 31 Aug 2021 02:53:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4966b0df9406b7041e14316e04c9579806832fafa02c5d3bd1842163b7f2353a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.11_9.tar.gz';          ;;        armhf|armv7l)          ESUM='2d7aba0b9ea287145ad437d4b3035fc84f7508e78c6fec99be4ff59fe1b6fc0d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.11_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='945b114bd0a617d742653ac1ae89d35384bf89389046a44681109cf8e4f4af91';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.11_9.tar.gz';          ;;        s390x)          ESUM='5d81979d27d9d8b3ed5bca1a91fc899cbbfb3d907f445ee7329628105e92f52c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.11_9.tar.gz';          ;;        amd64|x86_64)          ESUM='e99b98f851541202ab64401594901e583b764e368814320eba442095251e78cb';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.11_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:53:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:53:29 GMT
CMD ["jshell"]
# Tue, 31 Aug 2021 05:56:07 GMT
ARG MAVEN_VERSION=3.8.2
# Tue, 31 Aug 2021 05:56:08 GMT
ARG USER_HOME_DIR=/root
# Tue, 31 Aug 2021 05:56:08 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Tue, 31 Aug 2021 05:56:09 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Tue, 31 Aug 2021 05:56:30 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:56:41 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 31 Aug 2021 05:56:41 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 31 Aug 2021 05:56:42 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 31 Aug 2021 05:56:42 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 31 Aug 2021 05:56:43 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 31 Aug 2021 05:56:43 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 31 Aug 2021 05:56:44 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b915f774c910de28b940b41c37fc76946eb150ac0a4048d2d2cbc5b3b0983c26`  
		Last Modified: Tue, 31 Aug 2021 02:59:59 GMT  
		Size: 14.9 MB (14902564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d02c85e01bf1e58da064c6dafcb84948e5f14c7c0e2e309a17dbc73d08becb`  
		Last Modified: Tue, 31 Aug 2021 03:02:32 GMT  
		Size: 181.7 MB (181746352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541510ddfee4e14444386bf4549f4c5617f98e3d8bc195dc4b28cfa2859b1fcb`  
		Last Modified: Tue, 31 Aug 2021 06:00:51 GMT  
		Size: 27.3 MB (27292408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52109ac0dea9846d2ef30ec9fead394745119d699869fd81f217bf8345ed81`  
		Last Modified: Tue, 31 Aug 2021 06:00:37 GMT  
		Size: 9.4 MB (9405458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76b4e20a34243e2bd14bc464e075ab145a75ad92d8cd633f0caec51fabe4d89`  
		Last Modified: Tue, 31 Aug 2021 06:00:34 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a16ef3de91c3d68524f77d2fe56cd45e71528978835ab9e8bd7e78dbd033a`  
		Last Modified: Tue, 31 Aug 2021 06:00:34 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk-11` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:d20cf1e709588aef37a9c035b3225b797f49a79379b786add1bc63d11f1516ca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.1 MB (274056822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef59d3b708c5573a6a338efbede5d59a5dac30b3a9724e3da6824db3bba6100`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 01:59:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 01:59:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:59:55 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Tue, 31 Aug 2021 02:00:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4966b0df9406b7041e14316e04c9579806832fafa02c5d3bd1842163b7f2353a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.11_9.tar.gz';          ;;        armhf|armv7l)          ESUM='2d7aba0b9ea287145ad437d4b3035fc84f7508e78c6fec99be4ff59fe1b6fc0d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.11_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='945b114bd0a617d742653ac1ae89d35384bf89389046a44681109cf8e4f4af91';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.11_9.tar.gz';          ;;        s390x)          ESUM='5d81979d27d9d8b3ed5bca1a91fc899cbbfb3d907f445ee7329628105e92f52c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.11_9.tar.gz';          ;;        amd64|x86_64)          ESUM='e99b98f851541202ab64401594901e583b764e368814320eba442095251e78cb';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.11_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:00:06 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:00:07 GMT
CMD ["jshell"]
# Tue, 31 Aug 2021 03:46:49 GMT
ARG MAVEN_VERSION=3.8.2
# Tue, 31 Aug 2021 03:46:49 GMT
ARG USER_HOME_DIR=/root
# Tue, 31 Aug 2021 03:46:49 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Tue, 31 Aug 2021 03:46:49 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Tue, 31 Aug 2021 03:46:59 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:01 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 31 Aug 2021 03:47:01 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 31 Aug 2021 03:47:02 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 31 Aug 2021 03:47:02 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 31 Aug 2021 03:47:02 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 31 Aug 2021 03:47:02 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 31 Aug 2021 03:47:02 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75cf2699e7a04f04b6453d3cb46b19df309b905e083a05e30e31c4269c859c6`  
		Last Modified: Tue, 31 Aug 2021 02:03:12 GMT  
		Size: 15.9 MB (15898384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc5f10c5eb2606a0b8414aa91a8dee1ff699306a3803b0592f605e0fc477f00`  
		Last Modified: Tue, 31 Aug 2021 02:04:16 GMT  
		Size: 190.4 MB (190379257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831a7e28c07119a77a31a795a3627b081ef86843548e82d61a9d15568fe9da4b`  
		Last Modified: Tue, 31 Aug 2021 03:53:23 GMT  
		Size: 31.2 MB (31199407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da8683593b3ec255029d355ec87d3afef4aeb4b82cc1fc8ddb629ba62a3750c`  
		Last Modified: Tue, 31 Aug 2021 03:53:19 GMT  
		Size: 9.4 MB (9405463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2098eda861467ce61897dcef7b993fea7be4400c54432e9386699eab7181e37`  
		Last Modified: Tue, 31 Aug 2021 03:53:18 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0236eef04464749a1fb85c09452c324792c4cf494b559230ed43a76f7955f937`  
		Last Modified: Tue, 31 Aug 2021 03:53:18 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk-11` - linux; ppc64le

```console
$ docker pull maven@sha256:9f822aa44b127d5fed5e9ee081052592f6e285d3563b0a468abb8d7a5886e62e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.8 MB (273823973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68cfae999b14d818e66bb89e91276611ec3224edb831473c6cd423355fe51621`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:29:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 27 Jul 2021 02:31:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:32:05 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Tue, 27 Jul 2021 02:32:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4966b0df9406b7041e14316e04c9579806832fafa02c5d3bd1842163b7f2353a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.11_9.tar.gz';          ;;        armhf|armv7l)          ESUM='2d7aba0b9ea287145ad437d4b3035fc84f7508e78c6fec99be4ff59fe1b6fc0d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.11_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='945b114bd0a617d742653ac1ae89d35384bf89389046a44681109cf8e4f4af91';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.11_9.tar.gz';          ;;        s390x)          ESUM='5d81979d27d9d8b3ed5bca1a91fc899cbbfb3d907f445ee7329628105e92f52c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.11_9.tar.gz';          ;;        amd64|x86_64)          ESUM='e99b98f851541202ab64401594901e583b764e368814320eba442095251e78cb';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.11_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 27 Jul 2021 02:32:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 27 Jul 2021 02:32:25 GMT
CMD ["jshell"]
# Mon, 16 Aug 2021 17:20:47 GMT
ARG MAVEN_VERSION=3.8.2
# Mon, 16 Aug 2021 17:20:52 GMT
ARG USER_HOME_DIR=/root
# Mon, 16 Aug 2021 17:21:02 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Mon, 16 Aug 2021 17:21:08 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Mon, 16 Aug 2021 17:23:07 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:23:27 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 16 Aug 2021 17:23:37 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 16 Aug 2021 17:23:46 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 16 Aug 2021 17:23:48 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 16 Aug 2021 17:23:51 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 16 Aug 2021 17:23:55 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 16 Aug 2021 17:24:02 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629a3a6202ba14277a2a950fe566401dab14c010da680a9c37344d8481a8eae`  
		Last Modified: Tue, 27 Jul 2021 02:47:46 GMT  
		Size: 17.2 MB (17208945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009c2b1f241f48ef89a3e4fd11d0192010f6f27b738c53845e3e9aba77263b50`  
		Last Modified: Tue, 27 Jul 2021 02:48:44 GMT  
		Size: 175.5 MB (175549355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d917741195169f8b3b2b2a0c23955dfb5df437c38fd90dfc5fe8af9323044780`  
		Last Modified: Mon, 16 Aug 2021 17:53:16 GMT  
		Size: 38.4 MB (38368565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619d2ae5c01dbfa480978e73cca49bfb88606fd4567adbf1cbacc76a03978523`  
		Last Modified: Mon, 16 Aug 2021 17:53:09 GMT  
		Size: 9.4 MB (9405465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a820d7d977001045f1bda986aa52ae6cbedb3bca4076776187a377c956a182`  
		Last Modified: Mon, 16 Aug 2021 17:53:07 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d0b70db204c5670f96b0c512412cb3b32b1b4ea3caf919ba428a88c2ec0dc9`  
		Last Modified: Mon, 16 Aug 2021 17:53:08 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk-11` - linux; s390x

```console
$ docker pull maven@sha256:76d098a587dbee78a964a5bc149190b94b3f66bd133cbe166f58febaa9954cd4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.5 MB (251548379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e080cf8932acc32af39e2cc248cdad5d87ba4d00aac20952809f8dbdfa43063b`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:07:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 02:08:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:09:02 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Tue, 31 Aug 2021 02:09:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4966b0df9406b7041e14316e04c9579806832fafa02c5d3bd1842163b7f2353a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.11_9.tar.gz';          ;;        armhf|armv7l)          ESUM='2d7aba0b9ea287145ad437d4b3035fc84f7508e78c6fec99be4ff59fe1b6fc0d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.11_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='945b114bd0a617d742653ac1ae89d35384bf89389046a44681109cf8e4f4af91';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.11_9.tar.gz';          ;;        s390x)          ESUM='5d81979d27d9d8b3ed5bca1a91fc899cbbfb3d907f445ee7329628105e92f52c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.11_9.tar.gz';          ;;        amd64|x86_64)          ESUM='e99b98f851541202ab64401594901e583b764e368814320eba442095251e78cb';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.11_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:09:21 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:09:21 GMT
CMD ["jshell"]
# Tue, 31 Aug 2021 03:02:13 GMT
ARG MAVEN_VERSION=3.8.2
# Tue, 31 Aug 2021 03:02:13 GMT
ARG USER_HOME_DIR=/root
# Tue, 31 Aug 2021 03:02:14 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Tue, 31 Aug 2021 03:02:14 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Tue, 31 Aug 2021 03:02:30 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:02:44 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 31 Aug 2021 03:02:45 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 31 Aug 2021 03:02:45 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 31 Aug 2021 03:02:45 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 31 Aug 2021 03:02:46 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 31 Aug 2021 03:02:46 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 31 Aug 2021 03:02:46 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f47f4732fca5d50031ca6edf4776dd30d7e8eda1569ec50c3463d649acfc210`  
		Last Modified: Tue, 31 Aug 2021 02:23:22 GMT  
		Size: 15.7 MB (15741639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19bcb63eebf11bb1997d963ba346f16056541fb8441784733b2f91cd4d015b9`  
		Last Modified: Tue, 31 Aug 2021 02:24:00 GMT  
		Size: 168.6 MB (168589011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0287c2314c8ce4fad4c7691bcb88907d2e7bf78e4ab6d1c34ca90533eafad2d`  
		Last Modified: Tue, 31 Aug 2021 03:08:22 GMT  
		Size: 30.7 MB (30683580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3057ff00ba73aa843baac0eb38dddc210d8cd0cb15067a00b5a1dd3183619d41`  
		Last Modified: Tue, 31 Aug 2021 03:08:17 GMT  
		Size: 9.4 MB (9405466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3f59da2a0cf68253e2e8ac827f9e5af91f8dfad4b68ade0cc5f569eef4afb7`  
		Last Modified: Tue, 31 Aug 2021 03:08:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0556915e9168d48be83b97290adba070be7585d805326aca5199e8364b7649`  
		Last Modified: Tue, 31 Aug 2021 03:08:17 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
