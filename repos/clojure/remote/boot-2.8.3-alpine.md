## `clojure:boot-2.8.3-alpine`

```console
$ docker pull clojure@sha256:c43189da0c5e5fe3a1d965a72b855930917b76e92c28f5800ee68189e1102d83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:boot-2.8.3-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:43ac984e7e0dddcae443f2d439c0a6ac019c6119a4dc2d383e2a1e5895be1b32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.0 MB (265992267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a22d0f95ecd7ffb13958761806971909bb9526c6112accbf08e6f7cc51a0b6`
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
# Wed, 24 Aug 2022 19:21:34 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 24 Aug 2022 19:21:58 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1a1706304c26da0d8d2e05127c5aa7dba00e5401b2c0228c8ae894d2812beee0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Wed, 24 Aug 2022 19:22:01 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 19:22:01 GMT
CMD ["jshell"]
# Wed, 24 Aug 2022 21:52:09 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 24 Aug 2022 21:52:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 24 Aug 2022 21:52:09 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 21:52:10 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Wed, 24 Aug 2022 21:52:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 24 Aug 2022 21:52:10 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 24 Aug 2022 21:52:28 GMT
RUN boot
# Wed, 24 Aug 2022 21:52:29 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 24 Aug 2022 21:52:29 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 24 Aug 2022 21:52:29 GMT
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
	-	`sha256:baeea62e55107d5bcc912b1129b9a5e2551f65b996d4b613a8293615d39d04f4`  
		Last Modified: Wed, 24 Aug 2022 19:28:44 GMT  
		Size: 191.5 MB (191455735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf13604fb49c89ab5f868ccdf7c54522e7dd3f0639fc4e927a8c49026f1304`  
		Last Modified: Wed, 24 Aug 2022 19:28:29 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d740fd2a5e802dafd3a0ef2869fc9c73b31ae5d9982ae97a7b516c9cf37dfd`  
		Last Modified: Wed, 24 Aug 2022 21:59:52 GMT  
		Size: 859.3 KB (859318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1cf4a72276722448e64be3803a18ea7ebab54d013045399e195889615c8310`  
		Last Modified: Wed, 24 Aug 2022 21:59:55 GMT  
		Size: 58.8 MB (58820510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785d38c58294f814fe2904df5fd3926afa3780ddb22dcf35d26f6b5073bf3cf8`  
		Last Modified: Wed, 24 Aug 2022 21:59:52 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
