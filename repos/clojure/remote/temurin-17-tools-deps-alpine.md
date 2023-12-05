## `clojure:temurin-17-tools-deps-alpine`

```console
$ docker pull clojure@sha256:4d147916005970f3d24d29000f3e54374cec6aed4f38eb06056e1c856e2cf40b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-17-tools-deps-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:ed20eb5278cda133811a35e592847644a93b6da339f9b41fb160ff530ed5a80d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187862302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:767606325d52c667657d0796496241c0839feeb7fcf0c20cc59abe6cd669ba33`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:11:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 01 Dec 2023 07:11:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Dec 2023 07:11:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 01 Dec 2023 07:12:38 GMT
RUN set -eux;     apk add --no-cache         bash         fontconfig ttf-dejavu         java-cacerts         libretls zlib         musl-locales musl-locales-lang         binutils         tzdata     ;     rm -rf /var/cache/apk/*
# Fri, 01 Dec 2023 07:12:38 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Fri, 01 Dec 2023 07:12:47 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='c2a571a56e5bd3f30956b17b048880078c7801ed9e8754af6d1e38b9176059a9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Fri, 01 Dec 2023 07:12:50 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Fri, 01 Dec 2023 07:12:50 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 01 Dec 2023 07:12:50 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 01 Dec 2023 07:12:50 GMT
CMD ["jshell"]
# Tue, 05 Dec 2023 18:28:47 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:28:48 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:28:52 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Tue, 05 Dec 2023 18:28:53 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:28:53 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 05 Dec 2023 18:28:53 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 05 Dec 2023 18:28:53 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5820a814e8c90e2b86457ad1da29a79516ae242489d7bf67ea216d150c1efdc`  
		Last Modified: Fri, 01 Dec 2023 07:15:58 GMT  
		Size: 13.1 MB (13141060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec533064323b9596a959f12635ca06c4ee0965ca1b44257c3e65fca566a63512`  
		Last Modified: Fri, 01 Dec 2023 07:16:08 GMT  
		Size: 144.1 MB (144111197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb67c9837c6a071b2db6278557e6372b3cd1049dbf05b46970ebcd3462a542a2`  
		Last Modified: Fri, 01 Dec 2023 07:15:57 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f3195d8bdd8ee99ecf37259027c679b512a94c32c26bc7e461556da58f8d99`  
		Last Modified: Fri, 01 Dec 2023 07:15:57 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c243977dffd57d503573130fe4a3a1aef08de7c49352a843a5f884b9d426fd`  
		Last Modified: Tue, 05 Dec 2023 18:40:18 GMT  
		Size: 27.2 MB (27205689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217268ef8021caa9d57be80533a81799c9a2e334b30d03c6de6da1d5974eec4`  
		Last Modified: Tue, 05 Dec 2023 18:40:16 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c645a6ee99f14a5a43afecbdb6c5cecbf8668f0d111c79f16a8407f9ecf17fc`  
		Last Modified: Tue, 05 Dec 2023 18:40:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
