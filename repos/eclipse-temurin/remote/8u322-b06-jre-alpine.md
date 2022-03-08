## `eclipse-temurin:8u322-b06-jre-alpine`

```console
$ docker pull eclipse-temurin@sha256:fa61c455af0100c2746549acabc7ca1bef9c74274aafd9885828f88cbefb1abf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eclipse-temurin:8u322-b06-jre-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:74afe513d0a5c96b2c46ed2a01db2fbadbd5559514e5d8ac1e76341069863f5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44985796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5862348c095eec3973bbfc8e2749db367c1296955318d0db0e1c699d2d0835`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 17:19:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 13 Jan 2022 17:19:46 GMT
RUN apk add --no-cache tzdata musl-locales musl-locales-lang     && rm -rf /var/cache/apk/*
# Tue, 08 Mar 2022 20:26:38 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Tue, 08 Mar 2022 20:27:01 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='984f1a1f96774e6fbb644031b89de349afb354c9d12232ffb500c6a5d4013b1b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_alpine-linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 08 Mar 2022 20:27:02 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Mar 2022 20:27:02 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7418fdfb53d3b677d087a50df49ad12829a9eab2f0b2c8c19b162589387891`  
		Last Modified: Thu, 13 Jan 2022 17:22:44 GMT  
		Size: 430.3 KB (430278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3540d43b143e24702f42be71d2362c96f16ecc1c62b97e3a11683cb353624a87`  
		Last Modified: Tue, 08 Mar 2022 20:29:49 GMT  
		Size: 41.7 MB (41736943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4d160f1be8538513088a13590c640af69fe6553bbfc1803fb1293387bc6362`  
		Last Modified: Tue, 08 Mar 2022 20:29:42 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
