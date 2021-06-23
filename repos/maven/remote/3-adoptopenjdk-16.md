## `maven:3-adoptopenjdk-16`

```console
$ docker pull maven@sha256:dde5e2708d3efdb78812a5fb5f989721246885c5e1a1fe52a1ffa24c6acb1c15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-adoptopenjdk-16` - linux; amd64

```console
$ docker pull maven@sha256:b8aa23010dfca2b4be70287b746e025134cb9d757ad1475f7748011c0d02b1e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.8 MB (291840259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bb5929b61c3abf923e8cab9e821af05c56783edf97ef27d8b137c9adafd00fb`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:28:46 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 18 Jun 2021 00:29:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:30:35 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Fri, 18 Jun 2021 00:30:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3447ec27a6dbd4f3a6180a0d4371bb09aa428c16eea9983e515a7400cc9f5c85';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='20fc395d8ea2659e6407cd4ec233dc4399f61b7610f3a16495deb23c1e3b81df';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8d8e35ca5a7e24f16384bf32b110562921c19b4cfe65969980937bf879462bc6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='421cd44661cdbf0c2da79ab3104c81a1fa171b974038e55b1b3d4a042865588f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='7fdda042207efcedd30cd76d6295ed56b9c2e248cb3682c50898a560d4aa1c6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Jun 2021 00:30:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Jun 2021 00:30:47 GMT
CMD ["jshell"]
# Fri, 18 Jun 2021 06:05:40 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 18 Jun 2021 06:05:41 GMT
ARG USER_HOME_DIR=/root
# Fri, 18 Jun 2021 06:05:41 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 18 Jun 2021 06:05:41 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 18 Jun 2021 06:05:49 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 06:05:51 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 18 Jun 2021 06:05:52 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 18 Jun 2021 06:05:52 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 18 Jun 2021 06:05:52 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 18 Jun 2021 06:05:52 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 18 Jun 2021 06:05:52 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 18 Jun 2021 06:05:53 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7766c75e8fade5c21578ec8566d2929e7238f9ac1dbe88551bf2f147b76c65`  
		Last Modified: Fri, 18 Jun 2021 00:39:29 GMT  
		Size: 16.0 MB (16033037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e45d3be1f6235ea254c1f369afd60cfc69ad64da24e047d67acfcc29b857cf4`  
		Last Modified: Fri, 18 Jun 2021 00:42:03 GMT  
		Size: 206.5 MB (206472159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5ec57d6166d18f4a2a46706fcee3fe5b35a529a908ef45f97690c3dbc85ef6`  
		Last Modified: Fri, 18 Jun 2021 06:11:02 GMT  
		Size: 31.2 MB (31169204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d93c9e005d6525863bc5da0a227da514865449da0ca6ffad630c91e15911553`  
		Last Modified: Fri, 18 Jun 2021 06:10:58 GMT  
		Size: 9.6 MB (9610954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d094c9dbb8fc918d13a52f414c90ce2e1de00181b4fdfabaa51c37c20bd4c43d`  
		Last Modified: Fri, 18 Jun 2021 06:10:57 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf4fc483ced674ab5feb9a5d6e53942bacc6bb823fe2477540145c0ee1e2f32`  
		Last Modified: Fri, 18 Jun 2021 06:10:57 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk-16` - linux; arm variant v7

```console
$ docker pull maven@sha256:51816192ac118a45bc8353cc081760a47bf449329bcd0c05dbbf36f10a90fb43
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.6 MB (264553919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62c2c7357797aa11b40c0beb0ceba5927a7aa8c7d8634eec6530b9bc5d2393c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Sat, 03 Apr 2021 01:42:07 GMT
ADD file:76d0a7f82466172411203f4c90d7ec41979ea48db42fa3dd8a53f15622612f6e in / 
# Sat, 03 Apr 2021 01:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 01:42:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 01:42:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 01:42:15 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:59:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 02:59:58 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 03:01:41 GMT
ENV JAVA_VERSION=jdk-16+36
# Sat, 03 Apr 2021 03:02:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7217a9f9be3b0c8dfc78538f95fd2deb493eb651152d975062920566492b2574';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jdk_aarch64_linux_hotspot_16_36.tar.gz';          ;;        armhf|armv7l)          ESUM='f1d32ba01a40c98889f31368c0e987d6bbda65a7c50b8c088623b48e3a90104a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jdk_arm_linux_hotspot_16_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='07438952a22007c308440072cf3835c1c075e7102670cc666a3c47c8648da35a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jdk_ppc64le_linux_hotspot_16_36.tar.gz';          ;;        s390x)          ESUM='df34376116433f0e46c5e4935d73a0827d37b34d029f592d3b9383c92b024952';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jdk_s390x_linux_hotspot_16_36.tar.gz';          ;;        amd64|x86_64)          ESUM='2e031cf37018161c9e59b45fa4b98ff2ce4ce9297b824c512989d579a70f8422';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jdk_x64_linux_hotspot_16_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 03 Apr 2021 03:02:06 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 03 Apr 2021 03:02:07 GMT
CMD ["jshell"]
# Thu, 15 Apr 2021 18:59:44 GMT
ARG MAVEN_VERSION=3.8.1
# Thu, 15 Apr 2021 18:59:45 GMT
ARG USER_HOME_DIR=/root
# Thu, 15 Apr 2021 18:59:45 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Thu, 15 Apr 2021 18:59:46 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Thu, 15 Apr 2021 19:00:26 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Thu, 15 Apr 2021 19:00:32 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 15 Apr 2021 19:00:35 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 15 Apr 2021 19:00:35 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 15 Apr 2021 19:00:36 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 15 Apr 2021 19:00:38 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 15 Apr 2021 19:00:39 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 15 Apr 2021 19:00:39 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:2b310eb6279419eece82e847effefb67be66a3b8e631fda5532880177728460e`  
		Last Modified: Fri, 02 Apr 2021 12:47:42 GMT  
		Size: 24.0 MB (24048394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051c3059c680dcb64b0535e921132c5c74999d067a3eee05538c186b50546bb5`  
		Last Modified: Sat, 03 Apr 2021 01:44:02 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0927a80501a33ba38863296941a21c086fe86d55e066d7b4095548ef7e2a17e3`  
		Last Modified: Sat, 03 Apr 2021 01:44:01 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8525cbef9c7967df50e8b3c9ef5fa49eb36b70042ed2b15dc648ebe3a07dedd`  
		Last Modified: Sat, 03 Apr 2021 03:03:20 GMT  
		Size: 14.9 MB (14899076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8091bfdd4aa23620704d20087e1a4b32a9312b389be7e9d1d58642f360f48f66`  
		Last Modified: Sat, 03 Apr 2021 03:05:54 GMT  
		Size: 188.7 MB (188703052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e719fff5aaa0c7c8f2b7050fe49fcf6aebbffb5baf27e272a58553bb37d7df70`  
		Last Modified: Thu, 15 Apr 2021 19:01:10 GMT  
		Size: 27.3 MB (27290178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e693b55605dd5c428e166853ded7e8329f9e0d66ba64e00c48097640f8b4ec2`  
		Last Modified: Thu, 15 Apr 2021 19:01:03 GMT  
		Size: 9.6 MB (9610969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d78e68c43b09ba1876d47285c21332af057b354743fe95f73c84be52b33af5`  
		Last Modified: Thu, 15 Apr 2021 19:01:01 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccf2906b508d9380e6779cc788b30f657a174cd4296767aaac0463e54dcc048`  
		Last Modified: Thu, 15 Apr 2021 19:01:01 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk-16` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:a4c2a7de201d5072bc2308059801363d655ba260f195377cf0b6d661e7c84b61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.0 MB (287959490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf3c9b4685172c03a620d4fbb309158dde26e42897600caa06411e7af7157741`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:31:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 18 Jun 2021 00:31:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:32:59 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Fri, 18 Jun 2021 00:33:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3447ec27a6dbd4f3a6180a0d4371bb09aa428c16eea9983e515a7400cc9f5c85';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='20fc395d8ea2659e6407cd4ec233dc4399f61b7610f3a16495deb23c1e3b81df';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8d8e35ca5a7e24f16384bf32b110562921c19b4cfe65969980937bf879462bc6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='421cd44661cdbf0c2da79ab3104c81a1fa171b974038e55b1b3d4a042865588f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='7fdda042207efcedd30cd76d6295ed56b9c2e248cb3682c50898a560d4aa1c6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Jun 2021 00:33:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Jun 2021 00:33:10 GMT
CMD ["jshell"]
# Tue, 22 Jun 2021 23:02:07 GMT
ARG MAVEN_VERSION=3.8.1
# Tue, 22 Jun 2021 23:02:07 GMT
ARG USER_HOME_DIR=/root
# Tue, 22 Jun 2021 23:02:07 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Tue, 22 Jun 2021 23:02:07 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Tue, 22 Jun 2021 23:02:17 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Tue, 22 Jun 2021 23:02:24 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 22 Jun 2021 23:02:24 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 22 Jun 2021 23:02:24 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 22 Jun 2021 23:02:24 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 22 Jun 2021 23:02:24 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 22 Jun 2021 23:02:25 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 22 Jun 2021 23:02:25 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff470c6007f78550376884f4972cc5c767c6adc6f7d6002adddbddfb4600ea4b`  
		Last Modified: Fri, 18 Jun 2021 00:35:11 GMT  
		Size: 15.9 MB (15894169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132eceeaac158e1d7934011dcc1b9844906c6f43369765925945e08ee7b677e4`  
		Last Modified: Fri, 18 Jun 2021 00:38:01 GMT  
		Size: 204.1 MB (204094530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade03ae36c68a251c54e7306101aa5cf84a9f14fd5e627a83fdd8ec5af8358cc`  
		Last Modified: Tue, 22 Jun 2021 23:08:16 GMT  
		Size: 31.2 MB (31199813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b40fc6bd945395f58dea978747bac8f069d9e78cea76f67c0555f7e007bdcb`  
		Last Modified: Tue, 22 Jun 2021 23:08:10 GMT  
		Size: 9.6 MB (9610960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc20735ff09ec38644baace9a1ee68a68d1df231118311154cb9d90a31ef92d7`  
		Last Modified: Tue, 22 Jun 2021 23:08:09 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005829482eae4f56718af13fdaab6cdd2df099805f22ab10d25ea08a55f1da9b`  
		Last Modified: Tue, 22 Jun 2021 23:08:09 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk-16` - linux; ppc64le

```console
$ docker pull maven@sha256:f083e58e34a3bd068d341e0f58dc4ca6140b34a022137d114a68d354b7c95b1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.4 MB (285401392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:868b846b9aa526ca2228710c637e58780545ee1c83ca0efbdb3ee39bd715e025`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:29:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 18 Jun 2021 01:31:53 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:36:36 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Fri, 18 Jun 2021 01:37:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3447ec27a6dbd4f3a6180a0d4371bb09aa428c16eea9983e515a7400cc9f5c85';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='20fc395d8ea2659e6407cd4ec233dc4399f61b7610f3a16495deb23c1e3b81df';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8d8e35ca5a7e24f16384bf32b110562921c19b4cfe65969980937bf879462bc6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='421cd44661cdbf0c2da79ab3104c81a1fa171b974038e55b1b3d4a042865588f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='7fdda042207efcedd30cd76d6295ed56b9c2e248cb3682c50898a560d4aa1c6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Jun 2021 01:37:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Jun 2021 01:37:14 GMT
CMD ["jshell"]
# Fri, 18 Jun 2021 04:38:21 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 18 Jun 2021 04:38:25 GMT
ARG USER_HOME_DIR=/root
# Fri, 18 Jun 2021 04:38:28 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 18 Jun 2021 04:38:33 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 18 Jun 2021 04:40:06 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:40:22 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 18 Jun 2021 04:40:32 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 18 Jun 2021 04:40:38 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 18 Jun 2021 04:40:41 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 18 Jun 2021 04:40:46 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 18 Jun 2021 04:40:48 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 18 Jun 2021 04:40:52 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b268950217e490e209e0491ae6fbd3af12b4642aefad9c0039daf7b3ea0371`  
		Last Modified: Fri, 18 Jun 2021 01:52:43 GMT  
		Size: 17.2 MB (17208433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1647112d6f81f9ed44c7eb5783c5c811bbd13d392ba2c6bc021ec72890de70`  
		Last Modified: Fri, 18 Jun 2021 01:55:34 GMT  
		Size: 186.9 MB (186934016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612e3666175737251f07e5465d46e45211bfbecb1e9114c9069255fa21732d40`  
		Last Modified: Fri, 18 Jun 2021 04:50:01 GMT  
		Size: 38.4 MB (38368542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc477a79453061c96815bcc1a1f965419a50d21c756e6deb95c22f65383ca8e`  
		Last Modified: Fri, 18 Jun 2021 04:49:54 GMT  
		Size: 9.6 MB (9610948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81d6b1c4e0f23960a965c1b217eba70ef401d26261149bdf0e4a706d4677d46`  
		Last Modified: Fri, 18 Jun 2021 04:49:52 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67df812266d3982c213310396772a1c1c222c4ebfcaae50595d0195da7478a07`  
		Last Modified: Fri, 18 Jun 2021 04:49:52 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk-16` - linux; s390x

```console
$ docker pull maven@sha256:79ac7f721c3398df378459018f678c0d40d8809132bea81f32c46f3cf36753a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263011898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c9d07d18b728a4c347dbc67b1b54219b26ec23b890ae2ae1ca534c77aed26f0`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 17 Jun 2021 23:44:00 GMT
ADD file:737a08bab262cc2abc326912fdb8c8038222b272a5967b25ec6c761539c9d456 in / 
# Thu, 17 Jun 2021 23:44:02 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:09:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 18 Jun 2021 00:09:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:11:39 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Fri, 18 Jun 2021 00:11:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3447ec27a6dbd4f3a6180a0d4371bb09aa428c16eea9983e515a7400cc9f5c85';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='20fc395d8ea2659e6407cd4ec233dc4399f61b7610f3a16495deb23c1e3b81df';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8d8e35ca5a7e24f16384bf32b110562921c19b4cfe65969980937bf879462bc6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='421cd44661cdbf0c2da79ab3104c81a1fa171b974038e55b1b3d4a042865588f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='7fdda042207efcedd30cd76d6295ed56b9c2e248cb3682c50898a560d4aa1c6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Jun 2021 00:11:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Jun 2021 00:11:58 GMT
CMD ["jshell"]
# Fri, 18 Jun 2021 01:55:18 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 18 Jun 2021 01:55:19 GMT
ARG USER_HOME_DIR=/root
# Fri, 18 Jun 2021 01:55:19 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 18 Jun 2021 01:55:19 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 18 Jun 2021 01:55:27 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:55:40 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 18 Jun 2021 01:55:41 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 18 Jun 2021 01:55:41 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 18 Jun 2021 01:55:41 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 18 Jun 2021 01:55:42 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 18 Jun 2021 01:55:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 18 Jun 2021 01:55:42 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:be436b7e641e3737311249dadcc71ad61ba7bc9597248f426c58c8548cff8af0`  
		Last Modified: Thu, 17 Jun 2021 23:45:32 GMT  
		Size: 27.1 MB (27140902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92cd82b21097d2899d125e539a498d2f79c992bd6ebee596f4d3a3fc26dd7b6`  
		Last Modified: Fri, 18 Jun 2021 00:20:59 GMT  
		Size: 15.7 MB (15741691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07688acb393e8f0d582b9e34c27ce97f51116e539d4e119bf6e54d3a94942f1f`  
		Last Modified: Fri, 18 Jun 2021 00:22:41 GMT  
		Size: 179.8 MB (179834115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b3ab12f4aefb0e9d9d3336665b86b832a2253e8842c335280e1ad72136bd6d`  
		Last Modified: Fri, 18 Jun 2021 01:58:19 GMT  
		Size: 30.7 MB (30683027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1943c234059b82c61170a6d212662042a3a63e33eeeaecdc19da2dced6c3f7f`  
		Last Modified: Fri, 18 Jun 2021 01:58:15 GMT  
		Size: 9.6 MB (9610951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28cf0eb012c3c72452b4631157c74c4d86991c86f1a10d3a58b51cc716366ee`  
		Last Modified: Fri, 18 Jun 2021 01:58:14 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a856e7215c7e6a472def028520a81f032f2957943e9048e712ca1ace9bb03b0e`  
		Last Modified: Fri, 18 Jun 2021 01:58:14 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
