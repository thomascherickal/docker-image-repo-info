## `maven:3-adoptopenjdk-15`

```console
$ docker pull maven@sha256:c0ac9440e14748f73f4cf3e85adf4d02bef3da8476c14acf9398bddbd0dd7bbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-adoptopenjdk-15` - linux; amd64

```console
$ docker pull maven@sha256:86c82dbfa9cb413274734f39559bb74ed082e4361db91eb67e4e9cac5fcf81c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.4 MB (292418033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b653b7a7792d3821f4b8e0147388b81c0afd3812db89e020de3a62879f871657`
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
# Fri, 18 Jun 2021 00:30:08 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Fri, 18 Jun 2021 00:30:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Jun 2021 00:30:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Jun 2021 00:30:20 GMT
CMD ["jshell"]
# Fri, 18 Jun 2021 06:05:11 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 18 Jun 2021 06:05:11 GMT
ARG USER_HOME_DIR=/root
# Fri, 18 Jun 2021 06:05:12 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 18 Jun 2021 06:05:12 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 18 Jun 2021 06:05:20 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 06:05:27 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 18 Jun 2021 06:05:27 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 18 Jun 2021 06:05:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 18 Jun 2021 06:05:28 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 18 Jun 2021 06:05:28 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 18 Jun 2021 06:05:28 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 18 Jun 2021 06:05:28 GMT
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
	-	`sha256:452e61a70c96df9e622d81c5b07b5d0c8ec77e3cad689df1241c3757435cad09`  
		Last Modified: Fri, 18 Jun 2021 00:41:13 GMT  
		Size: 207.0 MB (207049749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52de0ad3501c0e7be374267d7c9f649146073a7a34325c2c0f7c4a8f1e3eb51f`  
		Last Modified: Fri, 18 Jun 2021 06:10:17 GMT  
		Size: 31.2 MB (31169374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7400a58d4e4a5c41d9215253a5f90459ac9a0f29568bd1d23899b44cd4ba39d7`  
		Last Modified: Fri, 18 Jun 2021 06:10:12 GMT  
		Size: 9.6 MB (9610970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f13af9d504dd3ae6644bb9f6bd015c4d6355914850d43e7ecad1d4df2944615`  
		Last Modified: Fri, 18 Jun 2021 06:10:11 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0cd0e210ca262443b3215ad7e7d973dc648390dc336b02619e51ab511f27f2`  
		Last Modified: Fri, 18 Jun 2021 06:10:11 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk-15` - linux; arm variant v7

```console
$ docker pull maven@sha256:92288c28b201873b8bfc4a33c6f90d972115337cfd89a6e9a43884a7fa5b0203
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.6 MB (266571511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128cbe689b4c4d2984f3370be8c408b4cc0df0916475a8958b8836ae5e7efd86`
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
# Sat, 03 Apr 2021 03:00:52 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Sat, 03 Apr 2021 03:01:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 03 Apr 2021 03:01:14 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 03 Apr 2021 03:01:14 GMT
CMD ["jshell"]
# Mon, 05 Apr 2021 16:59:56 GMT
ARG MAVEN_VERSION=3.8.1
# Mon, 05 Apr 2021 16:59:57 GMT
ARG USER_HOME_DIR=/root
# Mon, 05 Apr 2021 16:59:58 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Mon, 05 Apr 2021 16:59:58 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Mon, 05 Apr 2021 17:00:20 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Apr 2021 17:00:31 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 05 Apr 2021 17:00:32 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 05 Apr 2021 17:00:35 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 05 Apr 2021 17:00:36 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 05 Apr 2021 17:00:37 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 05 Apr 2021 17:00:37 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 05 Apr 2021 17:00:38 GMT
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
	-	`sha256:e434819f2b18cb8b7a3b6211fb08283c23136b837508efe7775bb66d657408c2`  
		Last Modified: Sat, 03 Apr 2021 03:04:48 GMT  
		Size: 190.7 MB (190720238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a510db762d2bbf41629d6df6f55eb7dfe157bc64acbf7ecf814508fe7b1fa045`  
		Last Modified: Mon, 05 Apr 2021 17:01:20 GMT  
		Size: 27.3 MB (27290589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b123fa04ea15cede244e6aa1734fbbf414409586447fdbe62411bedc2b904336`  
		Last Modified: Mon, 05 Apr 2021 17:01:13 GMT  
		Size: 9.6 MB (9610966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925140a3e7b0d0103f0aaa029ba1d8cc5278ccc735418beaea7b3abcfd601dbf`  
		Last Modified: Mon, 05 Apr 2021 17:01:12 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5fd620e9ac58cb89da428ab8460ec216969efbc9677c73c1fab1ec44561386`  
		Last Modified: Mon, 05 Apr 2021 17:01:12 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk-15` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:c2d4c52ee6ba6a4678161ee8a8ac49057f18e78d5199546f4c92f1f7c8ca1550
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288562722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa99f264c840743eb2783bda2e73ae51843a37bd51402fd1644a7788f61fd597`
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
# Fri, 18 Jun 2021 00:32:29 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Fri, 18 Jun 2021 00:32:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Jun 2021 00:32:39 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Jun 2021 00:32:39 GMT
CMD ["jshell"]
# Tue, 22 Jun 2021 23:01:35 GMT
ARG MAVEN_VERSION=3.8.1
# Tue, 22 Jun 2021 23:01:35 GMT
ARG USER_HOME_DIR=/root
# Tue, 22 Jun 2021 23:01:36 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Tue, 22 Jun 2021 23:01:36 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Tue, 22 Jun 2021 23:01:46 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Tue, 22 Jun 2021 23:01:53 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 22 Jun 2021 23:01:53 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 22 Jun 2021 23:01:53 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 22 Jun 2021 23:01:53 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 22 Jun 2021 23:01:54 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 22 Jun 2021 23:01:54 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 22 Jun 2021 23:01:54 GMT
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
	-	`sha256:ed3724d4239997a64d2c87e88c5872285a0ad578615207505cf08991bb9e556c`  
		Last Modified: Fri, 18 Jun 2021 00:37:04 GMT  
		Size: 204.7 MB (204697775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7d98bb03f0c5bbbdc686261f5f7e6d59a7280176dd575b4575139239c2dd8`  
		Last Modified: Tue, 22 Jun 2021 23:07:37 GMT  
		Size: 31.2 MB (31199800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebe128c2b8ddc85decf1e6231a037b812ac1968c46c5120b4008f166ef87fdc`  
		Last Modified: Tue, 22 Jun 2021 23:07:32 GMT  
		Size: 9.6 MB (9610962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd170a471af2c7ef24191e80a42337c24494d0b4e3fca945909a489575f0d197`  
		Last Modified: Tue, 22 Jun 2021 23:07:31 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0ca2dedf3833df2590f3584353b52f91d296f2fc5d9472715a851cee305b38`  
		Last Modified: Tue, 22 Jun 2021 23:07:31 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk-15` - linux; ppc64le

```console
$ docker pull maven@sha256:adfc149f4830d2fdc1888bb71005228106150794cf555066e388e194c41ca255
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.6 MB (287552398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:308c9a06713022202aea315f3146f27415a22ab16b6a265982f4eb0be55b0fa9`
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
# Fri, 18 Jun 2021 01:35:08 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Fri, 18 Jun 2021 01:35:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Jun 2021 01:35:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Jun 2021 01:35:50 GMT
CMD ["jshell"]
# Fri, 18 Jun 2021 04:34:40 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 18 Jun 2021 04:34:43 GMT
ARG USER_HOME_DIR=/root
# Fri, 18 Jun 2021 04:34:47 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 18 Jun 2021 04:34:51 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 18 Jun 2021 04:36:06 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:36:39 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 18 Jun 2021 04:36:47 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 18 Jun 2021 04:36:54 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 18 Jun 2021 04:36:59 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 18 Jun 2021 04:37:01 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 18 Jun 2021 04:37:07 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 18 Jun 2021 04:37:09 GMT
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
	-	`sha256:e2120fb5311c3194ef0e7e8ebddeb686eeddbfa52daadccfd747aadbac99e22d`  
		Last Modified: Fri, 18 Jun 2021 01:54:36 GMT  
		Size: 189.1 MB (189085158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834e07f5515b5eeddeb77cead5a43ff2a1429341e01ac3dfce5047405018d41d`  
		Last Modified: Fri, 18 Jun 2021 04:49:13 GMT  
		Size: 38.4 MB (38368394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4c5c184f80fa060b2d9e64913f27940ae6600e8042867e360fd4b9b8b01c`  
		Last Modified: Fri, 18 Jun 2021 04:49:06 GMT  
		Size: 9.6 MB (9610958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6734830f7e0c14593d20028802e86210c1807345bee8ae4ffcfcfb94b02aa37d`  
		Last Modified: Fri, 18 Jun 2021 04:49:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf17dc059cebeae6881380c93222e64e35967d04743d3ca8ecb7b18ed091b67`  
		Last Modified: Fri, 18 Jun 2021 04:49:04 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-adoptopenjdk-15` - linux; s390x

```console
$ docker pull maven@sha256:6b65f13feb5105cc39c987b871361a4926f0744844503e056cc3bd4dc5b79d17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.9 MB (263878605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff79228b4018818a0477d2dcdb934c908338ed800bedddd313a03e6e95215192`
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
# Fri, 18 Jun 2021 00:10:55 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Fri, 18 Jun 2021 00:11:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Jun 2021 00:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Jun 2021 00:11:17 GMT
CMD ["jshell"]
# Fri, 18 Jun 2021 01:54:49 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 18 Jun 2021 01:54:49 GMT
ARG USER_HOME_DIR=/root
# Fri, 18 Jun 2021 01:54:50 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 18 Jun 2021 01:54:50 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 18 Jun 2021 01:54:58 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:55:02 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 18 Jun 2021 01:55:02 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 18 Jun 2021 01:55:03 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 18 Jun 2021 01:55:03 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 18 Jun 2021 01:55:03 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 18 Jun 2021 01:55:03 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 18 Jun 2021 01:55:03 GMT
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
	-	`sha256:2842ee691c27f41b7532c7ee39ec5ee111d1c624fc61ec8a84e1e9b3d14c15b7`  
		Last Modified: Fri, 18 Jun 2021 00:22:06 GMT  
		Size: 180.7 MB (180701666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905365cf30fca8764280f72c1ddd9995f282571f6c893047e2830bf9c7b25e54`  
		Last Modified: Fri, 18 Jun 2021 01:57:54 GMT  
		Size: 30.7 MB (30682175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e89ff17781d6b4e1b763b2961d760738311b4ed64047a93d0397339ad1c618`  
		Last Modified: Fri, 18 Jun 2021 01:57:50 GMT  
		Size: 9.6 MB (9610960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bf5507bbe665e2b925931944eeee04dc8df6095f4275e9e465e3845b17e7a1`  
		Last Modified: Fri, 18 Jun 2021 01:57:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b5792bcdc7b135c057a38307ff576f618f398cd429a46fa9909aead0385199`  
		Last Modified: Fri, 18 Jun 2021 01:57:49 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
