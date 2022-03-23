## `eclipse-temurin:11-alpine`

```console
$ docker pull eclipse-temurin@sha256:c8a7873f8d39d4d592d7a33bdd24cc0b0c575faf506bf0d625bfe749d1b0bcbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eclipse-temurin:11-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:b8c709576af518a4ddc4200ca3b7b01b69f99cc7f07cc6eccfb148cec3ac5785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196135008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08018190f2f5b1fc235f99ee6e142bccf47a5b3a9f6fa1a92acb41e63565ac3c`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:17:50 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 23 Mar 2022 16:17:51 GMT
RUN apk add --no-cache tzdata musl-locales musl-locales-lang     && rm -rf /var/cache/apk/*
# Wed, 23 Mar 2022 16:18:30 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Wed, 23 Mar 2022 16:18:52 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='99e13a167ac27fac3dbfcc394a024fd9f4d84d24734ad5c250f97215d496ee36';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 23 Mar 2022 16:18:52 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 16:18:53 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 23 Mar 2022 16:18:53 GMT
CMD ["jshell"]
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
	-	`sha256:195ba304e5b8da75e5879b2547440fdc035a88cb4517b6cc6bce773d484252c7`  
		Last Modified: Wed, 23 Mar 2022 16:23:24 GMT  
		Size: 192.9 MB (192891709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992dc4fd27cbc26c8f34a7c80121122200838c1a4d9433887c1d6d9782a4e09e`  
		Last Modified: Wed, 23 Mar 2022 16:23:10 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
