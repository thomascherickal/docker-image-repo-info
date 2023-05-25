## `maven:3-eclipse-temurin-20-alpine`

```console
$ docker pull maven@sha256:7b255e62e09561d2f91f86547ab897a245d3a120b3caed2049cb0eaa5fe79dab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `maven:3-eclipse-temurin-20-alpine` - linux; amd64

```console
$ docker pull maven@sha256:221ee3b1055e92980f9f7ca954d71d9460347d61a0a87cfc8206181b75bbca6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.2 MB (225205724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928428cbf500230c6615dac8a03de2b9356e49580736a564b3a9e5efe946342c`
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
# Wed, 24 May 2023 23:36:20 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 24 May 2023 23:36:31 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='68d0f0c468064e944e304cab64fc162335d4d9bc0ddab7e6ff7a395a0bceda74';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jdk_x64_alpine-linux_hotspot_20.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 24 May 2023 23:36:33 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 24 May 2023 23:36:33 GMT
CMD ["jshell"]
# Wed, 24 May 2023 23:36:33 GMT
RUN apk add --no-cache bash procps curl tar # buildkit
# Wed, 24 May 2023 23:36:33 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 24 May 2023 23:36:33 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Wed, 24 May 2023 23:36:33 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Wed, 24 May 2023 23:36:33 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Wed, 24 May 2023 23:36:33 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Wed, 24 May 2023 23:36:33 GMT
ARG MAVEN_VERSION=3.9.2
# Wed, 24 May 2023 23:36:33 GMT
ARG USER_HOME_DIR=/root
# Wed, 24 May 2023 23:36:33 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 24 May 2023 23:36:33 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 24 May 2023 23:36:33 GMT
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
	-	`sha256:d186be75a39a7ec043f2add72ad6814c49f3c9ff69ce6fa723ed848ef20ddac6`  
		Last Modified: Wed, 24 May 2023 23:39:48 GMT  
		Size: 202.0 MB (201970839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e526c10d697363d272e3e97c106d942ec98c9d945118367b6a9e4fb16550400`  
		Last Modified: Wed, 24 May 2023 23:39:35 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631588a45a03caa7d87f92517f694f485845a46235458b2d97abba0343348ed2`  
		Last Modified: Thu, 25 May 2023 00:25:02 GMT  
		Size: 2.9 MB (2872991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4322169f8301883b0d122d9ba1d89de479fc34267f94213ea37a417ab579b4e0`  
		Last Modified: Thu, 25 May 2023 00:25:03 GMT  
		Size: 9.3 MB (9314429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a12fdd2e8541e10b0fc8095882001e4522eaa24caebbadbb34006a92f29526`  
		Last Modified: Thu, 25 May 2023 00:25:02 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d487648da95f7ea6377aee25f09beba3bf14499911f04f5d067b87e98325a97`  
		Last Modified: Thu, 25 May 2023 00:25:02 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b31f88dbfc5df97d67ec8b88e307cc87dd804d95de4ec7ea96635c972ac13fb`  
		Last Modified: Thu, 25 May 2023 00:25:02 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
