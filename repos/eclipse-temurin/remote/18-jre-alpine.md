## `eclipse-temurin:18-jre-alpine`

```console
$ docker pull eclipse-temurin@sha256:fbe0c7e7f167d3210ba36371fb0eb2f4ba2b1ed9e2e4a0d80c31cae6fd3d7e5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eclipse-temurin:18-jre-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:f49cd96a9441100488e873ac89701f8c0bb0098db142d923109fe9270a1f55a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49646678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a744f4273cd4046eeccbe00003baf84a79efe0bf5280e585d9feb48af83947a0`
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
# Wed, 08 Jun 2022 18:22:46 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 08 Jun 2022 18:23:25 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4362a13e81456ce66bc0f8c057e9ce964267a357573d5ccd15e9c955619c68f3';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_alpine-linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 08 Jun 2022 18:23:25 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Jun 2022 18:23:26 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:b7242960466216b60e3ebae4faf19843828d20418546ab7e58665dee7549b2bb`  
		Last Modified: Wed, 08 Jun 2022 18:28:01 GMT  
		Size: 46.4 MB (46401514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e5d1169831ca7d201737a13c5bbb282f4eac9e71cf763a27c5fdbf3633b15`  
		Last Modified: Wed, 08 Jun 2022 18:27:54 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
