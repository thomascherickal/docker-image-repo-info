## `eclipse-temurin:8u322-b06-jdk-alpine`

```console
$ docker pull eclipse-temurin@sha256:e872e7016cd88806c615dc77b47a46f036c217b0deeeb27afbbac822848ec62c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eclipse-temurin:8u322-b06-jdk-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:9a743b5ff8ad7da1b32bd45a96e0304fc9b5da600e4e838b4db7a4fc8b2d5009
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104822174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ffe250a84a424a0315694ed5486765121cf5229d1fc6ae3996dc50b03365d7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:17:50 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 23 Mar 2022 16:17:51 GMT
RUN apk add --no-cache tzdata musl-locales musl-locales-lang     && rm -rf /var/cache/apk/*
# Wed, 23 Mar 2022 16:17:51 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Wed, 23 Mar 2022 16:18:07 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='c7e781064c4a63ad6cd2399b2fa34de854a7d9bfd3ad2543d34bd7ba8f818822';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_alpine-linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 23 Mar 2022 16:18:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 16:18:08 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c36a4dbbc65cb1597970eac3f40685a2c565932a25f7450159034c46086a04`  
		Last Modified: Wed, 23 Mar 2022 16:22:29 GMT  
		Size: 430.4 KB (430449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849bf247abbea2ebe621e4ed9f6fe7701bcd0dfe878e4655a5b7112f0f2ca225`  
		Last Modified: Wed, 23 Mar 2022 16:22:38 GMT  
		Size: 101.6 MB (101578875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8aed2a025581bd317caddba9cadbba842dc268194ccc00a0b3f5bcef7a0661`  
		Last Modified: Wed, 23 Mar 2022 16:22:29 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
