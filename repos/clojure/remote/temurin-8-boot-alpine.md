## `clojure:temurin-8-boot-alpine`

```console
$ docker pull clojure@sha256:bc3126f672a146e8e541e4ad803931ce0de727d3fd70a2e02f3a8e141681aff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-8-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:eec9081d1c1e8d1f67134bb6d529c18ce35ed2795aa6911b0977b2d9e17b418b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.0 MB (175973024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c472bae45ccf78555729ca9c6193684ceb1a7fdd04c46224938c1189e05c6f1a`
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
# Thu, 06 Oct 2022 20:28:53 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 06 Oct 2022 20:29:02 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e5dcb8f947b687597f92fa80c008a2a17ce86f739dd6dce7ca741921621acb21';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_alpine-linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Thu, 06 Oct 2022 20:29:04 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Fri, 07 Oct 2022 05:04:10 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 07 Oct 2022 05:04:10 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 07 Oct 2022 05:04:11 GMT
WORKDIR /tmp
# Fri, 07 Oct 2022 05:04:12 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Fri, 07 Oct 2022 05:04:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 07 Oct 2022 05:04:12 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 07 Oct 2022 05:04:57 GMT
RUN boot
# Fri, 07 Oct 2022 05:04:58 GMT
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
	-	`sha256:9adf2ae612f0fdeadc30ca06d593860ee9f917b0a935973bf1ac559b9ee6c97a`  
		Last Modified: Thu, 06 Oct 2022 20:33:31 GMT  
		Size: 101.4 MB (101436607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c1c3768c2a194e624640b5d240dbd6b41300522e86a2d6fe22eca8de323f12`  
		Last Modified: Thu, 06 Oct 2022 20:33:23 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ce72e237deab59331f67e4b4f7881887bddf72dfce731c64b77b93180dcec9`  
		Last Modified: Fri, 07 Oct 2022 05:13:28 GMT  
		Size: 859.3 KB (859327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fd1be266a0abceba96a2e4e51acc1894807b8c8193bd4ff7dfad6b84b3d81e`  
		Last Modified: Fri, 07 Oct 2022 05:13:32 GMT  
		Size: 58.8 MB (58820802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
