## `clojure:boot-alpine`

```console
$ docker pull clojure@sha256:a36c416cca63af10809e2bc816008ccf8f2a5e5abcdd3997193825a5d5355343
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:f606084024e579999dbdc2e99405cce50a4c4327f88bf769c9c4fac6c1539a9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.0 MB (265983082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6ffb989894ff6695e9b633618e88ba21146c362bd4414f7226d26d0752f19fb`
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
# Fri, 07 Oct 2022 16:54:38 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Fri, 07 Oct 2022 16:54:57 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1a1706304c26da0d8d2e05127c5aa7dba00e5401b2c0228c8ae894d2812beee0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Fri, 07 Oct 2022 16:55:00 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 07 Oct 2022 16:55:00 GMT
CMD ["jshell"]
# Fri, 07 Oct 2022 17:20:18 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 07 Oct 2022 17:20:18 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 07 Oct 2022 17:20:18 GMT
WORKDIR /tmp
# Fri, 07 Oct 2022 17:20:19 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Fri, 07 Oct 2022 17:20:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 07 Oct 2022 17:20:19 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 07 Oct 2022 17:20:41 GMT
RUN boot
# Fri, 07 Oct 2022 17:20:42 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 07 Oct 2022 17:20:42 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 07 Oct 2022 17:20:42 GMT
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
	-	`sha256:66921d78a848ca667cee7c9ac5c36866360472568bff11508ec830e2cae8c513`  
		Last Modified: Fri, 07 Oct 2022 16:59:38 GMT  
		Size: 191.5 MB (191455720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9397d1cfc90c1e218a7afa7e2f30af6e85ccd47bd28f0d677d278019b0ed86da`  
		Last Modified: Fri, 07 Oct 2022 16:59:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc820a0b1bbe665f0f26708b19070fcf650ff71f7fce217e588b68fabbec6802`  
		Last Modified: Fri, 07 Oct 2022 17:27:34 GMT  
		Size: 858.8 KB (858804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c069927e2a0429288eb977c10b180479cf56915a78fcd5da9786398c66c150`  
		Last Modified: Fri, 07 Oct 2022 17:27:37 GMT  
		Size: 58.8 MB (58820586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc305fbaeb4a85851a232bc9272ffdc6ad015d8e10f6829b21f7dfb1734d5497`  
		Last Modified: Fri, 07 Oct 2022 17:27:34 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
