## `clojure:temurin-11-boot-alpine`

```console
$ docker pull clojure@sha256:c9206c48b088cabd06a34706cd731875d09ea2e6688d343c5cdb5ee68323007b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-11-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:f2526ad846fbd4089be18449ca222338b278d2e735bfb99418c9418c28e96072
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.0 MB (267994134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78cecd597c92de9934ecc89e3c646e35875bb476036cc550aa58580d112aff5d`
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
# Thu, 06 Oct 2022 20:29:27 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Thu, 06 Oct 2022 20:29:43 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='327b3bfd1c14e15bf6c7fb4d0c6c3f9406c1282a16e24b1424215d764f687cb6';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Thu, 06 Oct 2022 20:29:46 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 06 Oct 2022 20:29:46 GMT
CMD ["jshell"]
# Fri, 07 Oct 2022 05:06:06 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 07 Oct 2022 05:06:06 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 07 Oct 2022 05:06:07 GMT
WORKDIR /tmp
# Fri, 07 Oct 2022 05:06:08 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Fri, 07 Oct 2022 05:06:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 07 Oct 2022 05:06:08 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 07 Oct 2022 05:06:44 GMT
RUN boot
# Fri, 07 Oct 2022 05:06:44 GMT
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
	-	`sha256:5a8213774d127e423ef5255ac5c1720bd1da1a9c36c7ed56a16f8a1a57abdebb`  
		Last Modified: Thu, 06 Oct 2022 20:34:20 GMT  
		Size: 193.5 MB (193457703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d627f410c650341d2e659417865dc63d6073a245f2993b6f7c4cb2575c789080`  
		Last Modified: Thu, 06 Oct 2022 20:34:06 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03db89f80050b76bf99eb6630fe0c004767119cec75dc83069119166c792fc1d`  
		Last Modified: Fri, 07 Oct 2022 05:14:22 GMT  
		Size: 859.3 KB (859322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd1352828d605d31b3003d2ead4093f1278f7cc5b19fa85b2d1fb03d3e50c4d`  
		Last Modified: Fri, 07 Oct 2022 05:14:25 GMT  
		Size: 58.8 MB (58820804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
