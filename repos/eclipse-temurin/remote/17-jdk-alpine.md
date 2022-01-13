## `eclipse-temurin:17-jdk-alpine`

```console
$ docker pull eclipse-temurin@sha256:54e6d113aa6d80390a56fb1f62fe6e8600d0560b85cb774282d86f65956ed146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eclipse-temurin:17-jdk-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:9ae87d9dc6defd8f3b688d317f3bcb0ece6a2abb79e85dfce519e11ea2108fd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.1 MB (195104005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cd6d85814f336b7f504a5a36a1f1326a50501e8a8f03c9540f14933bec101c`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 17:19:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 13 Jan 2022 17:19:46 GMT
RUN apk add --no-cache tzdata musl-locales musl-locales-lang     && rm -rf /var/cache/apk/*
# Thu, 13 Jan 2022 17:20:54 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Thu, 13 Jan 2022 17:21:11 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='da4845987b3348da14338a0620ef7db25870e27670e82baebcc367fa9d17c7de';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 13 Jan 2022 17:21:12 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Jan 2022 17:21:13 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 13 Jan 2022 17:21:13 GMT
CMD ["jshell"]
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
	-	`sha256:926adebbf5f6f03ef62c167682da36f2806806c41121d722c0d3425ffe3ad846`  
		Last Modified: Thu, 13 Jan 2022 17:24:23 GMT  
		Size: 191.9 MB (191855155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fb9f484b7dd799eb9d09de4a52c613809db86906165ce47e268827cfa8c238`  
		Last Modified: Thu, 13 Jan 2022 17:24:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
