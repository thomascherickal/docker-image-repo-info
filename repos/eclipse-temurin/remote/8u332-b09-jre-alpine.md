## `eclipse-temurin:8u332-b09-jre-alpine`

```console
$ docker pull eclipse-temurin@sha256:214a135015055d996999e85e76d26f1aa152577c9009f465f1a02f39885a7422
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eclipse-temurin:8u332-b09-jre-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:f6485e494f9927cb6a51e23134b3556c62c32c3df20fc4317f7f493343726977
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45004124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b5b9beb371df196171c9851f3cab19b400315467860bc4b59b91f019e0a08c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:55:43 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 08 Jun 2022 18:20:30 GMT
RUN apk add --no-cache libretls musl-locales musl-locales-lang tzdata zlib     && rm -rf /var/cache/apk/*
# Wed, 08 Jun 2022 18:20:30 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Wed, 08 Jun 2022 18:21:05 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='58d584ac185c21ce8e90124cdfdf29621c7af52ac8a4e3aa9bdb08d53249a7f4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_x64_alpine-linux_hotspot_8u332b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 08 Jun 2022 18:21:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Jun 2022 18:21:05 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611b459a9f120c9f22143fbef6dda47c621957b1c86d4cbdf8fe3d9c762d728`  
		Last Modified: Wed, 08 Jun 2022 18:25:04 GMT  
		Size: 430.4 KB (430445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aea14557a82e943cf796fdf2deda96027076f12b86ef2fd1adc421d91da2516`  
		Last Modified: Wed, 08 Jun 2022 18:25:34 GMT  
		Size: 41.8 MB (41758960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7c91ae80cd6fbffffacfdbf443f6b7eb1b203ead030d80c7e17298c210876f`  
		Last Modified: Wed, 08 Jun 2022 18:25:28 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
