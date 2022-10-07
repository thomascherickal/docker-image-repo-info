## `clojure:temurin-11-boot-alpine`

```console
$ docker pull clojure@sha256:7a6890eb9da36cee2edc306f30024094edc29f48a00ac0f9066908d98592e81d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-11-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:634694d65a3c19ede9057177115725733b2c9162cd13cd27a9e88f07be7e7fa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.0 MB (267984748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81818930bd8daf096827201256ab2c9df8065e828ba60c99f7e33e269336c69a`
-	Default Command: `["boot","repl"]`

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
# Fri, 07 Oct 2022 16:53:57 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Fri, 07 Oct 2022 16:54:12 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='327b3bfd1c14e15bf6c7fb4d0c6c3f9406c1282a16e24b1424215d764f687cb6';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Fri, 07 Oct 2022 16:54:15 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 07 Oct 2022 16:54:15 GMT
CMD ["jshell"]
# Fri, 07 Oct 2022 17:18:53 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 07 Oct 2022 17:18:53 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 07 Oct 2022 17:18:53 GMT
WORKDIR /tmp
# Fri, 07 Oct 2022 17:18:54 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Fri, 07 Oct 2022 17:18:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 07 Oct 2022 17:18:55 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 07 Oct 2022 17:19:21 GMT
RUN boot
# Fri, 07 Oct 2022 17:19:21 GMT
CMD ["boot" "repl"]
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
	-	`sha256:fba20fc96420980a5e92cbc17d7ed8001550d853c0f3a2d2edab1d439b9f8a12`  
		Last Modified: Fri, 07 Oct 2022 16:58:47 GMT  
		Size: 193.5 MB (193457737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be129b993c212fc41b64fa2d86dc4b12ba9c94eaced404bab46dc0c9d72544a`  
		Last Modified: Fri, 07 Oct 2022 16:58:33 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45a9ca1699562a35da18ce990119d0b0d3a3515100dec1b2d4aca2c03bb2889`  
		Last Modified: Fri, 07 Oct 2022 17:26:37 GMT  
		Size: 858.8 KB (858795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd601781d5fcc8592de977d3870aa073c1e58f5a7b729faafa7c1ebda9026fe5`  
		Last Modified: Fri, 07 Oct 2022 17:26:40 GMT  
		Size: 58.8 MB (58820644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
