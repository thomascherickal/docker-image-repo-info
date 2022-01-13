## `maven:3-eclipse-temurin-11-alpine`

```console
$ docker pull maven@sha256:989e4c33f56674e9f4c11432ffcc55defa6cebd213771f7a2a5c3781d32af3b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `maven:3-eclipse-temurin-11-alpine` - linux; amd64

```console
$ docker pull maven@sha256:061770542b6626ce3ef86ae27ab43e9dd86f2ae0ca512f3d591cef98210267f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.5 MB (207493502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e329aebe419bcfc1b22e0588f8cbc5c1f7f2f0b0c9711fad88f7b13bc99266`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 17:19:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 13 Jan 2022 17:19:46 GMT
RUN apk add --no-cache tzdata musl-locales musl-locales-lang     && rm -rf /var/cache/apk/*
# Thu, 13 Jan 2022 17:19:46 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Thu, 13 Jan 2022 17:20:00 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4216543c8eaa4b10475bbacb15bbda41e04ec5c8c57424b3303f60c36b8b362d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 13 Jan 2022 17:20:00 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Jan 2022 17:20:01 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 13 Jan 2022 17:20:02 GMT
CMD ["jshell"]
# Thu, 13 Jan 2022 17:54:42 GMT
ARG MAVEN_VERSION=3.8.4
# Thu, 13 Jan 2022 17:54:42 GMT
ARG USER_HOME_DIR=/root
# Thu, 13 Jan 2022 17:54:43 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Thu, 13 Jan 2022 17:54:43 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Thu, 13 Jan 2022 17:54:44 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN apk add --no-cache curl tar bash procps
# Thu, 13 Jan 2022 17:54:46 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 13 Jan 2022 17:54:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 13 Jan 2022 17:54:46 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 13 Jan 2022 17:54:47 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 13 Jan 2022 17:54:47 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 13 Jan 2022 17:54:47 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 13 Jan 2022 17:54:47 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7418fdfb53d3b677d087a50df49ad12829a9eab2f0b2c8c19b162589387891`  
		Last Modified: Thu, 13 Jan 2022 17:22:44 GMT  
		Size: 430.3 KB (430278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1993115706b25b859be16a93b6d93e96027504d28faa817c1ac0fe54b3b57dcc`  
		Last Modified: Thu, 13 Jan 2022 17:23:01 GMT  
		Size: 192.7 MB (192741979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7015f870ee28658c6dbfc3f7b7527837a3a007ac378b09c64558014bf0cc67`  
		Last Modified: Thu, 13 Jan 2022 17:22:44 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892a6c7a59b9777bfc68e33de85414ebe54af2f0de615fd9bff7fcddf7dda503`  
		Last Modified: Thu, 13 Jan 2022 17:57:05 GMT  
		Size: 2.4 MB (2391641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c26840ebfe602c944da45199f78151157993956c38cc2ecbf53ce5169493a76`  
		Last Modified: Thu, 13 Jan 2022 17:57:05 GMT  
		Size: 9.1 MB (9109823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d1e2d115a48dc92df033c77d698f7dc93d680f6264af62d1fe6c192994188d`  
		Last Modified: Thu, 13 Jan 2022 17:57:04 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803739d304dd1f0e51ff915628a37df9379226a28001626386499cabf0684568`  
		Last Modified: Thu, 13 Jan 2022 17:57:04 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
