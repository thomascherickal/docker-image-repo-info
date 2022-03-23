## `eclipse-temurin:8-jre-alpine`

```console
$ docker pull eclipse-temurin@sha256:071ae59ff9a735f09a7342290bc50435a1da882b3e9f4bbc8439682ad9421d3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eclipse-temurin:8-jre-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:d1cd449d9a1f825ff82891eb6e7baa9ca99ec9c9e3d5c8eca61101fd6925a69e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44980220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06d9b602ca9b88e656b3dfb55ace410d57dfcb4ef75a55ba35adc8be908429bc`
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
# Wed, 23 Mar 2022 16:18:23 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='984f1a1f96774e6fbb644031b89de349afb354c9d12232ffb500c6a5d4013b1b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_alpine-linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 23 Mar 2022 16:18:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 16:18:24 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:d9d0f9d8d8417dc4a585d97c91e997893d97a0ebfea8e27164fba024b39ce510`  
		Last Modified: Wed, 23 Mar 2022 16:22:58 GMT  
		Size: 41.7 MB (41736922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c9cd015f26f45111148498a8c74429dfd5ea4a0e70b8e4dbc8b011a6540ff8`  
		Last Modified: Wed, 23 Mar 2022 16:22:53 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
