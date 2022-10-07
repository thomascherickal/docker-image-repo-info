## `clojure:temurin-17-boot-alpine`

```console
$ docker pull clojure@sha256:9685e90292e156dcab5a9c988378c71157bdb996b7a0bcefe50565b17070f77b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-17-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:4e7caddc6df6f12f6fe04c05255656c19e0378ce8fd94ca4ea324b1595b821d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.0 MB (265992295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e210b3ef465abd963b86f77084f0208a60f7369712d430924449e7db9a6fd1`
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
# Thu, 06 Oct 2022 20:30:13 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Thu, 06 Oct 2022 20:30:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1a1706304c26da0d8d2e05127c5aa7dba00e5401b2c0228c8ae894d2812beee0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Thu, 06 Oct 2022 20:30:36 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 06 Oct 2022 20:30:36 GMT
CMD ["jshell"]
# Fri, 07 Oct 2022 05:08:05 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 07 Oct 2022 05:08:05 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 07 Oct 2022 05:08:05 GMT
WORKDIR /tmp
# Fri, 07 Oct 2022 05:08:06 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Fri, 07 Oct 2022 05:08:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 07 Oct 2022 05:08:06 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 07 Oct 2022 05:08:34 GMT
RUN boot
# Fri, 07 Oct 2022 05:08:34 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 07 Oct 2022 05:08:34 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 07 Oct 2022 05:08:35 GMT
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
	-	`sha256:8a3a51737823497694fa5e9cebe8b7707efca2ce0ea52b15e1dcbffd589f8ba2`  
		Last Modified: Thu, 06 Oct 2022 20:35:11 GMT  
		Size: 191.5 MB (191455681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcdd16d0f27ebf8ead3fe9595fe15276a8d0e98a678ba4678967f1da3440a32`  
		Last Modified: Thu, 06 Oct 2022 20:34:55 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5527b593c1884885fe420e6473b85cd11e6e73e72aecb4d96dd667b6c61c4f16`  
		Last Modified: Fri, 07 Oct 2022 05:15:05 GMT  
		Size: 859.3 KB (859321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573b7a8eaf9ef8fef3f7b8ab18e847102db380d65dd402386a73807094d26691`  
		Last Modified: Fri, 07 Oct 2022 05:15:08 GMT  
		Size: 58.8 MB (58820586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1145340c7673f06da33b99244981a9d025a4d5432d7195733f4c7f9799580229`  
		Last Modified: Fri, 07 Oct 2022 05:15:05 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
