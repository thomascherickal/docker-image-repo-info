## `maven:eclipse-temurin-18-alpine`

```console
$ docker pull maven@sha256:e0faf73026823d8f74cdd35a1d7ffe6e0b14880193f7890b6c334ab407c69b21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `maven:eclipse-temurin-18-alpine` - linux; amd64

```console
$ docker pull maven@sha256:ff34d4e58258e78259d8426742124155b7d5d6611b017d2eb68f412c53ddd2bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.1 MB (207148071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9151943adaebfb4187c0f87823e02b99e811061ce9cc21b39323b2f74b20a04c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:55:43 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 05 Apr 2022 10:55:44 GMT
RUN apk add --no-cache tzdata musl-locales musl-locales-lang     && rm -rf /var/cache/apk/*
# Wed, 06 Apr 2022 19:20:28 GMT
ENV JAVA_VERSION=jdk-18+36
# Wed, 06 Apr 2022 19:20:41 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='3078b537f63603ce16d4b6bbc4499b9c00df55ee933a99dcbcefe9b596e93eae';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_x64_alpine-linux_hotspot_18_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 06 Apr 2022 19:20:41 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 19:20:42 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 06 Apr 2022 19:20:42 GMT
CMD ["jshell"]
# Wed, 13 Apr 2022 20:51:50 GMT
RUN apk add --no-cache curl tar bash procps
# Wed, 13 Apr 2022 20:51:50 GMT
ARG MAVEN_VERSION=3.8.5
# Wed, 13 Apr 2022 20:51:50 GMT
ARG USER_HOME_DIR=/root
# Wed, 13 Apr 2022 20:51:50 GMT
ARG SHA=89ab8ece99292476447ef6a6800d9842bbb60787b9b8a45c103aa61d2f205a971d8c3ddfb8b03e514455b4173602bd015e82958c0b3ddc1728a57126f773c743
# Wed, 13 Apr 2022 20:51:51 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.5/binaries
# Wed, 13 Apr 2022 20:51:52 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.5/binaries MAVEN_VERSION=3.8.5 SHA=89ab8ece99292476447ef6a6800d9842bbb60787b9b8a45c103aa61d2f205a971d8c3ddfb8b03e514455b4173602bd015e82958c0b3ddc1728a57126f773c743 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 13 Apr 2022 20:51:52 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 13 Apr 2022 20:51:53 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 13 Apr 2022 20:51:53 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 13 Apr 2022 20:51:53 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 13 Apr 2022 20:51:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 13 Apr 2022 20:51:53 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3277e9a7631c57d573722746688faad867a5b43dda77316e369e08ba94b713d`  
		Last Modified: Tue, 05 Apr 2022 10:59:33 GMT  
		Size: 430.5 KB (430455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12e37c5d3029e16e47e2666b7c0a6804a77fdaa7b298aa293581b5ccd91a8f2`  
		Last Modified: Wed, 06 Apr 2022 19:22:54 GMT  
		Size: 192.8 MB (192786139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87de7a66de5397a9785ae7c047e8cd6ba454a5223f16e9998833beeb365eb9fb`  
		Last Modified: Wed, 06 Apr 2022 19:22:40 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524bc3ae9ce9ff41186c5af09ea4b661b1fb3d3b21b9b7290da6d2e67624dea3`  
		Last Modified: Wed, 13 Apr 2022 20:54:41 GMT  
		Size: 2.4 MB (2379185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3724e403ca5970f47594355fcb104faeb8ff6a928d10f065c790329ac946da69`  
		Last Modified: Wed, 13 Apr 2022 20:54:41 GMT  
		Size: 8.7 MB (8736362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b2ab186df99f8f18861c9633429c16a91ec605dd5b14984ca89841d0339cab`  
		Last Modified: Wed, 13 Apr 2022 20:54:40 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f32e6d2312ccabbe08a76c89d615b8f69d23caee8081f47cc48b48da8a381`  
		Last Modified: Wed, 13 Apr 2022 20:54:40 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
