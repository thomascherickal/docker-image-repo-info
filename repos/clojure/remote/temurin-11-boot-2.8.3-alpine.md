## `clojure:temurin-11-boot-2.8.3-alpine`

```console
$ docker pull clojure@sha256:10f713d46c7481133df7623a0a625dd6e8ba17095b664b48ab7bd8bfc7b835da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-11-boot-2.8.3-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:78cdda5f07d065cb7a3d2891eb2b4e083baf7305af355f146eb9264a6a582ec3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.0 MB (267993839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85bf92f57e3bd1f330275bba4ee721e9431081d8e00eb294a0a6d42826e5d55`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 19:19:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:19:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:19:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 19:19:40 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Wed, 24 Aug 2022 19:19:58 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 24 Aug 2022 19:20:14 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='327b3bfd1c14e15bf6c7fb4d0c6c3f9406c1282a16e24b1424215d764f687cb6';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Wed, 24 Aug 2022 19:20:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 19:20:17 GMT
CMD ["jshell"]
# Wed, 24 Aug 2022 21:48:55 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 24 Aug 2022 21:48:55 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 24 Aug 2022 21:48:56 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 21:48:57 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Wed, 24 Aug 2022 21:48:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 24 Aug 2022 21:48:57 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 24 Aug 2022 21:49:15 GMT
RUN boot
# Wed, 24 Aug 2022 21:49:16 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107abfa4a9656cc98051eebaf02de090526191f4d53ab3733605b34f84513224`  
		Last Modified: Thu, 11 Aug 2022 19:29:52 GMT  
		Size: 12.1 MB (12050073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29496409cb750e4cd34c0abc2a0af5d4a8c9983eb3a8de05281f672289d5fb1e`  
		Last Modified: Wed, 24 Aug 2022 19:25:48 GMT  
		Size: 193.5 MB (193457720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0469b5bbda2d25b40afdbe052d9452b8af0246a6fc7abcea846b5ff7512de5b8`  
		Last Modified: Wed, 24 Aug 2022 19:25:34 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464bcafe8860e701c990fc4a8037cacbbc34d0e0def05ecdf4720508f9f542a6`  
		Last Modified: Wed, 24 Aug 2022 21:57:30 GMT  
		Size: 859.3 KB (859321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1b2f22273293a49884688faacb5432153e1eeec84175343b047dc76ecc211c`  
		Last Modified: Wed, 24 Aug 2022 21:57:33 GMT  
		Size: 58.8 MB (58820492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
