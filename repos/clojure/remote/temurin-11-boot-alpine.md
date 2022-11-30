## `clojure:temurin-11-boot-alpine`

```console
$ docker pull clojure@sha256:60bd4270fac625db5b83dfbce6769efccf69c67a8eecfe158b96577b1cf719f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-11-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:69cb94fa83fa980cac3fb52fd7d709aa702b736a48d94ddaeb9b9df002b8c735
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.9 MB (268920449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a1a58304d6c03c9feb23f404645b563c39d3c0a559af87c72cfa7305d57e769`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Tue, 29 Nov 2022 20:19:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 29 Nov 2022 20:19:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Nov 2022 20:19:48 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 29 Nov 2022 20:19:50 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Tue, 29 Nov 2022 20:20:55 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Tue, 29 Nov 2022 20:21:05 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='774d5955c09893dda14e3eb0fd3e239a6b2cec58615fcf4ec68747260b6e1cc1';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Tue, 29 Nov 2022 20:21:08 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 29 Nov 2022 20:21:08 GMT
CMD ["jshell"]
# Tue, 29 Nov 2022 22:53:53 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 29 Nov 2022 22:53:54 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 29 Nov 2022 22:53:54 GMT
WORKDIR /tmp
# Tue, 29 Nov 2022 22:53:56 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Tue, 29 Nov 2022 22:53:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 29 Nov 2022 22:53:56 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 29 Nov 2022 22:54:34 GMT
RUN boot
# Tue, 29 Nov 2022 22:54:35 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e5acd5897d762b9a83758d4ceae374df7b8b0367a48cc14b8a00e33998b3bf`  
		Last Modified: Tue, 29 Nov 2022 20:26:18 GMT  
		Size: 12.0 MB (12020105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d6e82f832d7246992d482aae2b0128c0c41588f28ea2ee995a45ec441763fc`  
		Last Modified: Tue, 29 Nov 2022 20:27:41 GMT  
		Size: 193.8 MB (193812574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f2f14f4397117ef79007059975b5e4d8bf1c1578a319858f720369abca2a10`  
		Last Modified: Tue, 29 Nov 2022 20:27:27 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f13190aa114013a6ddefef49664632e7f10858a80008d873090c55e4158226`  
		Last Modified: Tue, 29 Nov 2022 23:01:15 GMT  
		Size: 896.0 KB (895981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa535e041cfbda8fce9d4ad7f7f2df8996ae4d9e21a52bb0d9a192dce94e9f`  
		Last Modified: Tue, 29 Nov 2022 23:01:19 GMT  
		Size: 58.8 MB (58820905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
