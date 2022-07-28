## `maven:3-eclipse-temurin-11-alpine`

```console
$ docker pull maven@sha256:773353cd5870f7ad2c2da27e2934587f2b9f7c07d7e5e57355e63eae131f4ca5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `maven:3-eclipse-temurin-11-alpine` - linux; amd64

```console
$ docker pull maven@sha256:813ce1df7393687a90470dc2d53c2346a5384455057e208d41c29b8a0b1ae2b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.1 MB (219108824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e6ccd5c52016b242e833853ded6574c0dba3ef7f7787c489ee0d8c9aba0126`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:20:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 28 Jul 2022 16:20:06 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Thu, 28 Jul 2022 16:20:06 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 28 Jul 2022 16:20:30 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='32a93bd824cf34ccdde0881699a41a12722b4d8ff1d57294b2add2102432759b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Jul 2022 16:20:31 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 16:20:32 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 28 Jul 2022 16:20:32 GMT
CMD ["jshell"]
# Thu, 28 Jul 2022 18:59:17 GMT
RUN apk add --no-cache curl tar bash procps
# Thu, 28 Jul 2022 18:59:17 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 28 Jul 2022 18:59:17 GMT
ARG USER_HOME_DIR=/root
# Thu, 28 Jul 2022 18:59:17 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 28 Jul 2022 18:59:17 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 28 Jul 2022 18:59:18 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 28 Jul 2022 18:59:19 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 28 Jul 2022 18:59:19 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 28 Jul 2022 18:59:19 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 28 Jul 2022 18:59:19 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 28 Jul 2022 18:59:19 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 28 Jul 2022 18:59:19 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2b3b9d0d1a1f972083dde62c850175d26be845971e3c96ff06c8145fbe2fd0`  
		Last Modified: Thu, 28 Jul 2022 16:25:19 GMT  
		Size: 12.1 MB (12050034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9875ccc97d0d48928ad5d42b8735e689578585611d1a6c20452e964c47b88a`  
		Last Modified: Thu, 28 Jul 2022 16:25:31 GMT  
		Size: 193.5 MB (193453364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406868a12245358d162f9abe43d4aa81d7989b363b311962d858f0a01d5341b`  
		Last Modified: Thu, 28 Jul 2022 16:25:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96ec3f9dc15ba32d806da046ae4564e1166f5de705f60d23f72afc3f25c586b`  
		Last Modified: Thu, 28 Jul 2022 19:02:52 GMT  
		Size: 2.1 MB (2065760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750dca2b0eaf0f68945fc4b04f04419fe6f3ee416648cb1c5dee4662bbe1fb73`  
		Last Modified: Thu, 28 Jul 2022 19:02:52 GMT  
		Size: 8.7 MB (8739487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162d7217d6ba67951bab3e4cce477c25dfd95c30084969ad50f00e946a05f5c3`  
		Last Modified: Thu, 28 Jul 2022 19:02:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ca0911ae12743a1085b34f51ed2043c035804068e93ec718d5aee6eda09aec`  
		Last Modified: Thu, 28 Jul 2022 19:02:52 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
