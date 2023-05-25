## `maven:3-eclipse-temurin-8-alpine`

```console
$ docker pull maven@sha256:a81dec99fc5bb4f5d06bdb9857267b3e8c3ee1ca0d7dc6f8a3ff4080b9b5b320
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `maven:3-eclipse-temurin-8-alpine` - linux; amd64

```console
$ docker pull maven@sha256:971c0e3a0ca46e572676bf55a0a1df1e4a8229a6e182d0f1b6f2bbb8c68cdc7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75774365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c321114aa70bf3b670ff624901909e5659a09e6665e218b3522e3dab4416e5bd`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 24 May 2023 23:34:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 24 May 2023 23:34:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 May 2023 23:34:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 24 May 2023 23:34:29 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Wed, 24 May 2023 23:34:29 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 24 May 2023 23:34:35 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='cfdf8e07c8eeb087b7a2895b90fc0a19986bcff85006f1e2b708e3964909aa8e';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_x64_alpine-linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 24 May 2023 23:34:36 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Wed, 24 May 2023 23:34:36 GMT
RUN apk add --no-cache bash procps curl tar # buildkit
# Wed, 24 May 2023 23:34:36 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 24 May 2023 23:34:36 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Wed, 24 May 2023 23:34:36 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Wed, 24 May 2023 23:34:36 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Wed, 24 May 2023 23:34:36 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Wed, 24 May 2023 23:34:36 GMT
ARG MAVEN_VERSION=3.9.2
# Wed, 24 May 2023 23:34:36 GMT
ARG USER_HOME_DIR=/root
# Wed, 24 May 2023 23:34:36 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 24 May 2023 23:34:36 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 24 May 2023 23:34:36 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdde4a302e0d0ee2ef6760bf84344d762835ef2d38d2a1a1062c7d038fe2615b`  
		Last Modified: Wed, 24 May 2023 23:37:36 GMT  
		Size: 7.6 MB (7648427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d694a2b7c16a77c50982c0d6c082b7283771de0ec5cc847bd355b7ab684aedc9`  
		Last Modified: Wed, 24 May 2023 23:37:40 GMT  
		Size: 52.5 MB (52539524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d54ff8e92ad62b25089a5c48736e5c228115778e74dc2155361eda232c376ae`  
		Last Modified: Wed, 24 May 2023 23:37:34 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8d44611ce2a714c8065b62b6ac769664827e1acd42696365764f2fd7219b71`  
		Last Modified: Thu, 25 May 2023 00:25:16 GMT  
		Size: 2.9 MB (2872957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd0db5f73271fee6aef4b925155c778d613eb75cb9eace26a481cb3d74d11f9`  
		Last Modified: Thu, 25 May 2023 00:25:16 GMT  
		Size: 9.3 MB (9314440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328f0def4eceda0a762f7926883d20a4a36bde23c3be534c82f85874490e3009`  
		Last Modified: Thu, 25 May 2023 00:25:15 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068a0bfd220195ffa00d6605573be10c45fffa1e091629a8cc6638079706da08`  
		Last Modified: Thu, 25 May 2023 00:25:15 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e641b9c799f4f0a4908518ae7fd3aa58ae8714dff1423acb6d0b811a13c64a`  
		Last Modified: Thu, 25 May 2023 00:25:15 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
