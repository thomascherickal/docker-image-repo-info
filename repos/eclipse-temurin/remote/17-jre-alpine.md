## `eclipse-temurin:17-jre-alpine`

```console
$ docker pull eclipse-temurin@sha256:3ebd237b71203b3c8f5e5e10fac036bd4cee4d77b683d3a2e28272855bb758b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eclipse-temurin:17-jre-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:4a570846da85f6bfda2ff840aabb08d8e83bcf7b3e440c25381f2359c52b6482
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49797927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa2c98c2028c93f95fe92011df53495ed072a394d6506294c5e50c3592edd6d3`
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
# Wed, 23 Mar 2022 16:20:42 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Wed, 23 Mar 2022 16:21:09 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='043b3169b3d1f6fbf0d807e61b9f94d167d08e13dd2f4fb76786e60ee65e5ae5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_alpine-linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 23 Mar 2022 16:21:09 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 16:21:10 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:d94c1c3405ba2b968d26bb4bc894b5fba02fcb50740d0bae5d5c386333984eb9`  
		Last Modified: Wed, 23 Mar 2022 16:25:04 GMT  
		Size: 46.6 MB (46554629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aed7bcc1f451a30040a9f3c369b8e948553a3fd9a6c390a6148af5b966e8335`  
		Last Modified: Wed, 23 Mar 2022 16:24:57 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
