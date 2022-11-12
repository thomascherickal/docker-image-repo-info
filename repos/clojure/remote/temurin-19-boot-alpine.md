## `clojure:temurin-19-boot-alpine`

```console
$ docker pull clojure@sha256:ec4542f564e63714b428aedae6cac23a2ff110782a1e3212b07a2593dccc2478
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-19-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:9e311d40804cd253bc2ea32629e1ccec0aa5373f4b8d63801a900d6dd2dfb7c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274820059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00b55607073f7314d7d4acd13caa0e9235e1cb8373411ad0174d2eae9f25eb5e`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:12:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 12 Nov 2022 05:12:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Nov 2022 05:12:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 12 Nov 2022 05:12:06 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Sat, 12 Nov 2022 05:14:15 GMT
ENV JAVA_VERSION=jdk-19.0.1+10
# Sat, 12 Nov 2022 05:14:35 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='76cfcdf47cdf24331b51939fd2840fd387cf62471da99e4718e2e42b486a9270';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_x64_alpine-linux_hotspot_19.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Sat, 12 Nov 2022 05:14:38 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 12 Nov 2022 05:14:38 GMT
CMD ["jshell"]
# Sat, 12 Nov 2022 10:36:58 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 12 Nov 2022 10:36:58 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 12 Nov 2022 10:36:58 GMT
WORKDIR /tmp
# Sat, 12 Nov 2022 10:36:59 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Sat, 12 Nov 2022 10:37:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 12 Nov 2022 10:37:00 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 12 Nov 2022 10:37:18 GMT
RUN boot
# Sat, 12 Nov 2022 10:37:18 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 12 Nov 2022 10:37:18 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 12 Nov 2022 10:37:19 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9822f87bb1185b1d8f81aa09fc8a20796bb3db4c90da28c6177e0fd8a3d8d3`  
		Last Modified: Sat, 12 Nov 2022 05:16:37 GMT  
		Size: 12.0 MB (12030631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f334dab74d0be632884d565506362427e88b3b8eda99949b482e665eb16228db`  
		Last Modified: Sat, 12 Nov 2022 05:19:12 GMT  
		Size: 200.3 MB (200303572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8636564591f925d6b7ffa028b7dfbfbf6a7350dc9a5aeb52d0597856e2c40a0`  
		Last Modified: Sat, 12 Nov 2022 05:18:57 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b238c215cab2e301bd14c856be69797d6468c283dc6d107cab03c511f3be6fe`  
		Last Modified: Sat, 12 Nov 2022 10:43:25 GMT  
		Size: 858.6 KB (858649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188a8ded948e733b8055d74451efebd62c5377a5609fcb8e0ad224caad420cb0`  
		Last Modified: Sat, 12 Nov 2022 10:43:28 GMT  
		Size: 58.8 MB (58820358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b23573786160924506b00da0fdb301d1e11d142115ac012992829e203042839`  
		Last Modified: Sat, 12 Nov 2022 10:43:25 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
