## `clojure:temurin-19-boot-2.8.3-alpine`

```console
$ docker pull clojure@sha256:d577a4b692e657c488a34a837fa94974d0022030af1081609793f20fb26efcac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-19-boot-2.8.3-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:09b6f5d04625f681cfb1d5fef8c91f5147393c26ed27dbed1a85cd8391a01fcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.6 MB (274568452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed027529d5a99c14901b2e1cf46497e65b811195a182dd44efb84f29ae3a410b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

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
# Fri, 07 Oct 2022 17:21:40 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 07 Oct 2022 17:21:40 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 07 Oct 2022 17:21:40 GMT
WORKDIR /tmp
# Fri, 07 Oct 2022 17:21:41 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Fri, 07 Oct 2022 17:21:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 07 Oct 2022 17:21:42 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 07 Oct 2022 17:22:02 GMT
RUN boot
# Fri, 07 Oct 2022 17:22:02 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 07 Oct 2022 17:22:02 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 07 Oct 2022 17:22:02 GMT
CMD ["repl"]
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
	-	`sha256:83e38235cfb6f434e0b5e64e88e7e1665c66c25dc0098f368d4e9b453212d020`  
		Last Modified: Fri, 07 Oct 2022 17:28:56 GMT  
		Size: 858.8 KB (858799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d248a2a73511481e927ddb34b21c522dc3a53ca91f75b5f216c8584155c312`  
		Last Modified: Fri, 07 Oct 2022 17:29:00 GMT  
		Size: 58.8 MB (58820387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a15fad9bd1d400fc5e8bb4cbfe4ed98fa2a94982c13eabf7940804a3f96482`  
		Last Modified: Fri, 07 Oct 2022 17:28:56 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
