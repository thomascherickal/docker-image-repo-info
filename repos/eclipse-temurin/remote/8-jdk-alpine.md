## `eclipse-temurin:8-jdk-alpine`

```console
$ docker pull eclipse-temurin@sha256:9c3fc9e095404d32f85c38129254296a700bde2dc3205818c23d8601fbdef9f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eclipse-temurin:8-jdk-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:ba13647ec8db0d514a668e45a0b0128674410c791e103f1de987a346f9133b4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104679043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:969b74322c8da076c3f492684e9c27c5d726f91446569b66e8d4520ca4ea6590`
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
# Wed, 08 Jun 2022 18:20:38 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='29705d2b619b40b0f3dbb05fa497b74851e872e4db6496c2b9b358e1dad967ff';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_alpine-linux_hotspot_8u332b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 08 Jun 2022 18:20:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Jun 2022 18:20:39 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:a19dc0c7040fdf8b28de159cf77ab41965834a3ebeef7a1ec055ddc127569835`  
		Last Modified: Wed, 08 Jun 2022 18:25:13 GMT  
		Size: 101.4 MB (101433878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ea2de2e163555121afcb091fa0987eb28477d0727426332cb773129c252976`  
		Last Modified: Wed, 08 Jun 2022 18:25:04 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
