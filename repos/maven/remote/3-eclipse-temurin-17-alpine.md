## `maven:3-eclipse-temurin-17-alpine`

```console
$ docker pull maven@sha256:261d7a5291198ced958c1d4927db3bc6c48095582b81d1814636153ae56c0c7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `maven:3-eclipse-temurin-17-alpine` - linux; amd64

```console
$ docker pull maven@sha256:3fa0155790749bd594666fd1229341c6ccd8a3c89fd5702e67880f69af45925b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.2 MB (206211426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7666849b40bbbdb0ef1138df88226153c9c7bce18df43bf942b397ec7d91f1`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 21 Jun 2022 20:21:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 21 Jun 2022 20:21:36 GMT
RUN apk add --no-cache libretls musl-locales musl-locales-lang tzdata zlib     && rm -rf /var/cache/apk/*
# Tue, 21 Jun 2022 20:22:54 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Tue, 21 Jun 2022 20:23:18 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='5cbaece6aec44f6d3911cfa3c5a8659889e85042aff214c944c5fa1b5938a5fc';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 21 Jun 2022 20:23:19 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Jun 2022 20:23:19 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 21 Jun 2022 20:23:19 GMT
CMD ["jshell"]
# Tue, 21 Jun 2022 21:27:24 GMT
RUN apk add --no-cache curl tar bash procps
# Tue, 21 Jun 2022 21:27:24 GMT
ARG MAVEN_VERSION=3.8.6
# Tue, 21 Jun 2022 21:27:24 GMT
ARG USER_HOME_DIR=/root
# Tue, 21 Jun 2022 21:27:24 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Tue, 21 Jun 2022 21:27:24 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Tue, 21 Jun 2022 21:27:32 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 21 Jun 2022 21:27:32 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 21 Jun 2022 21:27:32 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 21 Jun 2022 21:27:32 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 21 Jun 2022 21:27:32 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 21 Jun 2022 21:27:33 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 21 Jun 2022 21:27:33 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4177d2591259bff2bae6f43f12721dbe4ed5aac24fb0991377a3d27cdd534e`  
		Last Modified: Tue, 21 Jun 2022 20:26:07 GMT  
		Size: 477.8 KB (477755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192e69d5289dec2e5bbf3ed1456166acafdc67b3e657981604fa21df9ae64084`  
		Last Modified: Tue, 21 Jun 2022 20:27:54 GMT  
		Size: 191.8 MB (191809195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbdc495bee83415cd6c7ddec5b7a12d388962b684278496d8d5798a5a13cd90`  
		Last Modified: Tue, 21 Jun 2022 20:27:40 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be91c271c01743e027184f76bd7d9ad5a4290229ee04650af3dab13b813ebd22`  
		Last Modified: Tue, 21 Jun 2022 21:30:31 GMT  
		Size: 2.4 MB (2384735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a5dde51bb0bee821c4dee2417a8cecd34c6a2e49ad277b9bc061e19fbcee1b`  
		Last Modified: Tue, 21 Jun 2022 21:30:32 GMT  
		Size: 8.7 MB (8739480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9689642f552db378a6bcd1cd2139aebe98cd9b65caa9bc945055da7582408886`  
		Last Modified: Tue, 21 Jun 2022 21:30:31 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78624f6ec9c2dc85e8f838dfcdbeae48586d631efa5d02f7229aaaec784dbc7`  
		Last Modified: Tue, 21 Jun 2022 21:30:32 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
