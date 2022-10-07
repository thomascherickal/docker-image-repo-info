## `eclipse-temurin:19_36-jdk-alpine`

```console
$ docker pull eclipse-temurin@sha256:dd5b657f009864771e6906d0aa97f62f31481c3968946a1e7489fc8e0cc48cb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eclipse-temurin:19_36-jdk-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:77369ce3af440fee06d4c92baac27d28f720c7f5ea58590d0dd039c94e3a5b87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.9 MB (214888864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75489562208f9628e9662c658c90a066ad2db2bbef428cf7765f84a3ce64f91b`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 16:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 07 Oct 2022 16:53:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 16:53:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Oct 2022 16:53:21 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Fri, 07 Oct 2022 16:55:27 GMT
ENV JAVA_VERSION=jdk-19+36
# Fri, 07 Oct 2022 16:55:46 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='2a073c3cc977317baf7c0c4995be38d33e3ed74e9fa4ac075933016e68f18252';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jdk_x64_alpine-linux_hotspot_19_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Fri, 07 Oct 2022 16:55:49 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 07 Oct 2022 16:55:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5835cc7e6eb64b728c9694dd72d8aede877af0a2ec44f981847853af9abbf5`  
		Last Modified: Fri, 07 Oct 2022 16:57:51 GMT  
		Size: 12.0 MB (12041341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862e44a33ca79d5a7f3c2c7f6721a8c1ca58d24fb209c1cac5ca9a61c3902ce`  
		Last Modified: Fri, 07 Oct 2022 17:00:32 GMT  
		Size: 200.0 MB (200041295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6cbbd4fbc13d9b25eb5ece2353108b5979269f23f7bccb805f72feaf03bf66`  
		Last Modified: Fri, 07 Oct 2022 17:00:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
