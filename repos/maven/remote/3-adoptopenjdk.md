## `maven:3-adoptopenjdk`

```console
$ docker pull maven@sha256:bdf38193f4baaf4c608fde89878eb5262fe27188a6b6f9c49493614f3df1a733
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-adoptopenjdk` - linux; amd64

```console
$ docker pull maven@sha256:3defaff5aee2f1a033b2786d1c5a2dd4f0bef90f54551f8a20d6e6daa5d12ef4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.2 MB (292227857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53e4191ae0f0c63fa65a6bec2fc5939f43d7ddada016078200fc46917e394010`
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
# Mon, 26 Jul 2021 23:00:40 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Mon, 26 Jul 2021 23:00:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 26 Jul 2021 23:00:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 26 Jul 2021 23:00:50 GMT
CMD ["jshell"]
# Mon, 16 Aug 2021 17:27:14 GMT
ARG MAVEN_VERSION=3.8.2
# Mon, 16 Aug 2021 17:27:15 GMT
ARG USER_HOME_DIR=/root
# Mon, 16 Aug 2021 17:27:15 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Mon, 16 Aug 2021 17:27:15 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Mon, 16 Aug 2021 17:27:22 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:27:25 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 16 Aug 2021 17:27:25 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 16 Aug 2021 17:27:25 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 16 Aug 2021 17:27:25 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 16 Aug 2021 17:27:26 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 16 Aug 2021 17:27:26 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 16 Aug 2021 17:27:26 GMT
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
	-	`sha256:61e05c2132c8f80ffdef4dc3b26dce70948445d54f94078d32fbaeb86b63be89`  
		Last Modified: Mon, 26 Jul 2021 23:11:21 GMT  
		Size: 207.0 MB (207049773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e8a564c96f894d5d5ebefea46a7562b9263891015245bf018552c00936283`  
		Last Modified: Mon, 16 Aug 2021 17:37:08 GMT  
		Size: 31.2 MB (31170191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0afd593543690a2c47eab8420b4245d8e4c69aabd5a3955a431b5727a6178e2`  
		Last Modified: Mon, 16 Aug 2021 17:37:04 GMT  
		Size: 9.4 MB (9405472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a581f595acfbece0f1684117a99ff228f0cfd29371e411e9696e4b5bbeaa4034`  
		Last Modified: Mon, 16 Aug 2021 17:37:03 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687c1f950af2235b1bc95cf2cfd70c739f47f1462dedcea63132cc3b93a97647`  
		Last Modified: Mon, 16 Aug 2021 17:37:03 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk` - linux; arm variant v7

```console
$ docker pull maven@sha256:8f382de1c8bfd3e81a07f429995d55d6a9f1ff222fdd8096b2255af632d73f5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.4 MB (266390748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:210d240513279d4a74d4222b4f54393d97bdac09861d04c8a46c98b3caca2125`
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
# Tue, 31 Aug 2021 02:54:13 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Tue, 31 Aug 2021 02:54:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:54:42 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:54:43 GMT
CMD ["jshell"]
# Tue, 31 Aug 2021 05:56:56 GMT
ARG MAVEN_VERSION=3.8.2
# Tue, 31 Aug 2021 05:56:56 GMT
ARG USER_HOME_DIR=/root
# Tue, 31 Aug 2021 05:56:57 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Tue, 31 Aug 2021 05:56:57 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Tue, 31 Aug 2021 05:57:18 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:57:24 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 31 Aug 2021 05:57:25 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 31 Aug 2021 05:57:25 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 31 Aug 2021 05:57:26 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 31 Aug 2021 05:57:26 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 31 Aug 2021 05:57:27 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 31 Aug 2021 05:57:27 GMT
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
	-	`sha256:375ca2687a79aa6fee4f16aa55caa745e0e28bcd6c18186392cf5bd6ac174ee9`  
		Last Modified: Tue, 31 Aug 2021 03:04:42 GMT  
		Size: 190.7 MB (190720240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205551722f15d39cac6533809664323e21d26903c823c8989f4447f2cf18a4eb`  
		Last Modified: Tue, 31 Aug 2021 06:01:26 GMT  
		Size: 27.3 MB (27292455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ead39e4c08179b47d0ceae350f7cf49bc28b41d00a385ec59db6b79c85a0742`  
		Last Modified: Tue, 31 Aug 2021 06:01:11 GMT  
		Size: 9.4 MB (9405450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350314408502525018ce94b57c47d30cd0d0826323539a842736552af5aefc32`  
		Last Modified: Tue, 31 Aug 2021 06:01:08 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824023279c86a17ba41c69612ff2cc98ad7afc48864dc9a4c32da492dcb332ed`  
		Last Modified: Tue, 31 Aug 2021 06:01:08 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:8c33e25812963abfa058754df29a834049ee2d866487baf0c17d08060344ac86
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.4 MB (288375211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:675041165267d6fda17a2a6923f878560dadcb6ba72f26c618cd451b9a57ef83`
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
# Tue, 31 Aug 2021 02:00:25 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Tue, 31 Aug 2021 02:00:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:00:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:00:35 GMT
CMD ["jshell"]
# Tue, 31 Aug 2021 03:47:08 GMT
ARG MAVEN_VERSION=3.8.2
# Tue, 31 Aug 2021 03:47:09 GMT
ARG USER_HOME_DIR=/root
# Tue, 31 Aug 2021 03:47:09 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Tue, 31 Aug 2021 03:47:09 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Tue, 31 Aug 2021 03:47:18 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:27 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 31 Aug 2021 03:47:27 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 31 Aug 2021 03:47:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 31 Aug 2021 03:47:27 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 31 Aug 2021 03:47:27 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 31 Aug 2021 03:47:28 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 31 Aug 2021 03:47:28 GMT
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
	-	`sha256:be531d68c5f189a96fc5306152653f14cfd44ef510ce821ef2c5c98dad6342e5`  
		Last Modified: Tue, 31 Aug 2021 02:05:09 GMT  
		Size: 204.7 MB (204697682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e428a60ac76a346d9fca09f86a5bb973f7515e502de490b31e6b09c78e786cb`  
		Last Modified: Tue, 31 Aug 2021 03:53:44 GMT  
		Size: 31.2 MB (31199370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9674aa0e3ad964df7fcb51306c9b506933375f97101a5a598506e81b342619a7`  
		Last Modified: Tue, 31 Aug 2021 03:53:40 GMT  
		Size: 9.4 MB (9405463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a831074f7cb1affcfd05bd89105b5cd5ca9728693a5ce1d29ec33f3b3e1ea8`  
		Last Modified: Tue, 31 Aug 2021 03:53:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fcb6344a97f682c751562a0f1d39432d97742f6332e910fc90a8d2663057b3`  
		Last Modified: Tue, 31 Aug 2021 03:53:39 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk` - linux; ppc64le

```console
$ docker pull maven@sha256:a9f4380bd2d7e0c31647b08dc0cbe64dcfcac4baa9cc12a9473d77e95816c5a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.4 MB (287359863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f25039e25d8148c9e202af91a3d2b1b52aeeb94c9790fefe45d16dc3a1f2a3d7`
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
# Tue, 27 Jul 2021 02:33:00 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Tue, 27 Jul 2021 02:33:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 27 Jul 2021 02:33:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 27 Jul 2021 02:33:26 GMT
CMD ["jshell"]
# Mon, 16 Aug 2021 17:24:14 GMT
ARG MAVEN_VERSION=3.8.2
# Mon, 16 Aug 2021 17:24:21 GMT
ARG USER_HOME_DIR=/root
# Mon, 16 Aug 2021 17:24:27 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Mon, 16 Aug 2021 17:24:32 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Mon, 16 Aug 2021 17:26:20 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:26:35 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 16 Aug 2021 17:26:45 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 16 Aug 2021 17:26:50 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 16 Aug 2021 17:26:51 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 16 Aug 2021 17:26:53 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 16 Aug 2021 17:26:57 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 16 Aug 2021 17:27:02 GMT
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
	-	`sha256:ef0f44339b80d10d81604d94dd0225f69c8a6b796da41841bee55e043b4d9ef1`  
		Last Modified: Tue, 27 Jul 2021 02:49:39 GMT  
		Size: 189.1 MB (189085175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be0e43fafcb05429871dc29928f121552dd3d9627520165e901e267ab0377f2`  
		Last Modified: Mon, 16 Aug 2021 17:53:39 GMT  
		Size: 38.4 MB (38368641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549229b3da63e0609739deeca0e36befe2d3527c2d866a7cf76e02a2710b4062`  
		Last Modified: Mon, 16 Aug 2021 17:53:34 GMT  
		Size: 9.4 MB (9405460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99f68b9243f4bc71054ad0e6747244cc4f8d591a2c4b68e778dbb2900682288`  
		Last Modified: Mon, 16 Aug 2021 17:53:31 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed4ee9aa228a179c299314545e0d621dbc9ccba864daf99eba862e5418868f4`  
		Last Modified: Mon, 16 Aug 2021 17:53:31 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk` - linux; s390x

```console
$ docker pull maven@sha256:214064489c727dd857c294eed4293f770117629216362ed999ac40dc1be0ea0d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.7 MB (263661061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863d5ca9b58b0e1d65099846c5de84f18de9cf27be0f534f6737b43e5705662`
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
# Tue, 31 Aug 2021 02:09:47 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Tue, 31 Aug 2021 02:10:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:10:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:10:12 GMT
CMD ["jshell"]
# Tue, 31 Aug 2021 03:02:55 GMT
ARG MAVEN_VERSION=3.8.2
# Tue, 31 Aug 2021 03:02:55 GMT
ARG USER_HOME_DIR=/root
# Tue, 31 Aug 2021 03:02:56 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Tue, 31 Aug 2021 03:02:56 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Tue, 31 Aug 2021 03:03:08 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:03:21 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 31 Aug 2021 03:03:22 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 31 Aug 2021 03:03:22 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 31 Aug 2021 03:03:22 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 31 Aug 2021 03:03:23 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 31 Aug 2021 03:03:23 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 31 Aug 2021 03:03:23 GMT
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
	-	`sha256:30fa9dd1bf861ac7bf74d6d00671e6c26cd4a1c13eb260405cf941013481913d`  
		Last Modified: Tue, 31 Aug 2021 02:24:37 GMT  
		Size: 180.7 MB (180701656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed709bf59f6868309414f5472f8a1c6c965a07d873b9d1de9141ebed43ed7834`  
		Last Modified: Tue, 31 Aug 2021 03:08:36 GMT  
		Size: 30.7 MB (30683623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbf9f07ac3730f7ff8ff2114be34d33e856e73257abc817fc215391af10fe29`  
		Last Modified: Tue, 31 Aug 2021 03:08:32 GMT  
		Size: 9.4 MB (9405461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757b1d2cceba3e8ff8b898a40807078673c5abe6def0490508c747040e3a4926`  
		Last Modified: Tue, 31 Aug 2021 03:08:32 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b520de7479499954e08d05a82436748017e0c0c722651c7c57568def0e97b0`  
		Last Modified: Tue, 31 Aug 2021 03:08:31 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
