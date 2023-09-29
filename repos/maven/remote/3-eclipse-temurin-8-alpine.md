## `maven:3-eclipse-temurin-8-alpine`

```console
$ docker pull maven@sha256:a57bf9c28ad314e1c9d1239fbc0b6f883a1f6d1e14358f8a9044600c0a22314e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `maven:3-eclipse-temurin-8-alpine` - linux; amd64

```console
$ docker pull maven@sha256:804888c1ea2a54ab27e1361897f628d402744f6c562983d5d5974f552a15c5d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125419984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:275ca39765518e909275d125a1ddeeb7734bf10577465edd3fffb80ead33ab20`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 28 Sep 2023 23:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 23:24:24 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 28 Sep 2023 23:24:25 GMT
RUN apk add --no-cache fontconfig java-cacerts bash libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Thu, 28 Sep 2023 23:24:26 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Thu, 28 Sep 2023 23:24:31 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6cf2d4925c387c4cdc0bf2e71de3690527141b5244695d0b3109ce83a8512235';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_x64_alpine-linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Thu, 28 Sep 2023 23:24:32 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Thu, 28 Sep 2023 23:24:33 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Thu, 28 Sep 2023 23:24:33 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 18 Aug 2023 15:26:34 GMT
RUN apk add --no-cache bash procps curl tar # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
ARG MAVEN_VERSION=3.9.4
# Fri, 18 Aug 2023 15:26:34 GMT
ARG USER_HOME_DIR=/root
# Fri, 18 Aug 2023 15:26:34 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 18 Aug 2023 15:26:34 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 18 Aug 2023 15:26:34 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e4092d737c5d0c601ddadd8d075b756e55cc717065ae83683571965c2117a9`  
		Last Modified: Thu, 28 Sep 2023 23:28:20 GMT  
		Size: 9.3 MB (9276514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1076f6323c43e5087d2bb95d374dc7a408505995c17d3f38e5ddf3aa8774487`  
		Last Modified: Thu, 28 Sep 2023 23:28:28 GMT  
		Size: 101.5 MB (101488457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7530e3dbc8ddd8a31ebcf9a552cfee323caa314e496b064c11f5396d5bd9f80b`  
		Last Modified: Thu, 28 Sep 2023 23:28:19 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05429726b5869b70315ac86c634ec1babe60b99b3bad24c2e55a622663f586ac`  
		Last Modified: Thu, 28 Sep 2023 23:28:19 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc80a30f9d062c34b2d6ecfc0fe6d38e6d727abc882456af771d32c9d37611f5`  
		Last Modified: Fri, 29 Sep 2023 04:42:46 GMT  
		Size: 1.8 MB (1844353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2144cc86426c4cd010f758f8d6268bde2fc84304d8c69918c5eb44c60566e186`  
		Last Modified: Fri, 29 Sep 2023 04:42:47 GMT  
		Size: 9.4 MB (9406417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f545824b17ec3aa3a1a2bc4440c93626f824fefcbdfa193ac72753bfeb6b983`  
		Last Modified: Fri, 29 Sep 2023 04:42:46 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29b91d49e86f859faa09bb20823d50ad373590f60c296d67affd1677fcba2b1`  
		Last Modified: Fri, 29 Sep 2023 04:42:46 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203be338941872d90c13d9d03bc758e39354eccbbdccdb2b73bc96ab051571ea`  
		Last Modified: Fri, 29 Sep 2023 04:42:46 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
