## `clojure:temurin-17-boot-2.8.3-alpine`

```console
$ docker pull clojure@sha256:6ef9644d9f00f90efbc1072d47490f7ccfb76d3f2ba6ed91f04c29dca4e32357
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-17-boot-2.8.3-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:4a424cdab0f1535478f3fc0f9e75e1b8a0d0cc184896906c45726844e214121f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266253763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f9ce955d03d9dd17a95965138dc3cf8601ccf877c422d157158a0e76387e7e`
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
# Sat, 12 Nov 2022 05:13:30 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Sat, 12 Nov 2022 05:13:49 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='cb154396ff3bfb6a9082e3640c564643d31ecae1792fab0956149ed5258ad84b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Sat, 12 Nov 2022 05:13:51 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 12 Nov 2022 05:13:51 GMT
CMD ["jshell"]
# Sat, 12 Nov 2022 10:35:40 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 12 Nov 2022 10:35:40 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 12 Nov 2022 10:35:40 GMT
WORKDIR /tmp
# Sat, 12 Nov 2022 10:35:42 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Sat, 12 Nov 2022 10:35:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 12 Nov 2022 10:35:42 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 12 Nov 2022 10:36:00 GMT
RUN boot
# Sat, 12 Nov 2022 10:36:00 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 12 Nov 2022 10:36:00 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 12 Nov 2022 10:36:01 GMT
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
	-	`sha256:26dd5a4c9d9b66950c491bf46b0fa319e048043eee4d4f74a473b0f27cd70589`  
		Last Modified: Sat, 12 Nov 2022 05:18:22 GMT  
		Size: 191.7 MB (191737252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5b1b0a2ab2f3efa0b93fa43b3aa8d8ea84d62cf5dc6bd850464f5c14e2cef3`  
		Last Modified: Sat, 12 Nov 2022 05:18:07 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ceaddca5af25e477aa8ed905055ed89d747cffd570a8b87f61a1116089ff39b`  
		Last Modified: Sat, 12 Nov 2022 10:42:15 GMT  
		Size: 858.6 KB (858645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb2002f5e8edb1b28cf976dc138e92ba3f776e9b9c4633ee0071a675cbc4f3`  
		Last Modified: Sat, 12 Nov 2022 10:42:17 GMT  
		Size: 58.8 MB (58820383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e43af92ef26aad36aa57623e578112743f9239122db513b15cf00660f8d1`  
		Last Modified: Sat, 12 Nov 2022 10:42:14 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
