## `clojure:temurin-19-boot-2.8.3-alpine`

```console
$ docker pull clojure@sha256:544a846540d0c7a52f7aec612a96d2fd15f3de4766fd447dfdff0a605f96ca2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-19-boot-2.8.3-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:cc1b399f9676a0c7262671567055a670c47808146f4d595d6ff0e1fe1a449187
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.6 MB (274577812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8468e458e5174f92af933513523149de22e7cec1eb224ffb6ca347e9e4033a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

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
# Thu, 06 Oct 2022 20:31:02 GMT
ENV JAVA_VERSION=jdk-19+36
# Thu, 06 Oct 2022 20:31:20 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='2a073c3cc977317baf7c0c4995be38d33e3ed74e9fa4ac075933016e68f18252';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jdk_x64_alpine-linux_hotspot_19_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Thu, 06 Oct 2022 20:31:23 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 06 Oct 2022 20:31:23 GMT
CMD ["jshell"]
# Fri, 07 Oct 2022 05:09:37 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 07 Oct 2022 05:09:37 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 07 Oct 2022 05:09:37 GMT
WORKDIR /tmp
# Fri, 07 Oct 2022 05:09:38 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Fri, 07 Oct 2022 05:09:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 07 Oct 2022 05:09:39 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 07 Oct 2022 05:10:01 GMT
RUN boot
# Fri, 07 Oct 2022 05:10:01 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 07 Oct 2022 05:10:01 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 07 Oct 2022 05:10:01 GMT
CMD ["repl"]
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
	-	`sha256:173b4a2202f4ca0a7adc32480f38ca670587c90c0a6bbb3c31ffd9794483bb9b`  
		Last Modified: Thu, 06 Oct 2022 20:36:07 GMT  
		Size: 200.0 MB (200041317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7946ba95fd1f8d2bb7a22960f07d31e7cd0e51f79b06f7923eb974ed417a9a04`  
		Last Modified: Thu, 06 Oct 2022 20:35:52 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09746b32264668a8053e904c7af92a77fef952a2e25c65cdada47c3d5a95c617`  
		Last Modified: Fri, 07 Oct 2022 05:16:04 GMT  
		Size: 859.3 KB (859321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79651fca6933c334fbf3fe9e250be8ae035134e50bf207e71e9d4d5a140039f`  
		Last Modified: Fri, 07 Oct 2022 05:16:07 GMT  
		Size: 58.8 MB (58820468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c06c838d85632076ac3e19e178ba69a3ab2d14a2ea526a0a29bf274458bf650`  
		Last Modified: Fri, 07 Oct 2022 05:16:04 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
