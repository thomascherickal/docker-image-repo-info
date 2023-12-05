## `clojure:temurin-21-tools-deps-1.11.1.1429-alpine`

```console
$ docker pull clojure@sha256:7d3e858476f7820ed6c5bd30eb8b8eb4232a71a4c40ccc540f51797ad0ba4390
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-21-tools-deps-1.11.1.1429-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:e6884d0193cc28ea5f944f0e88948576fa365316838a56169875fcb110009b84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201416104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb293b5f491e424e0b5c021501912b0ab6feaf586fff34d97b133b8f828684b`
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
# Fri, 01 Dec 2023 07:13:19 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Fri, 01 Dec 2023 07:13:28 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='77006c0a753808c2a6662007906eb6eb230f2fb6eb9d201a39cc46113e68f82c';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_aarch64_alpine-linux_hotspot_21.0.1_12.tar.gz';          ;;        amd64|x86_64)          ESUM='422f23f5109056cacb9227247bebf8532e2dc3c9d505e71637ba610569d6b3ff';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_x64_alpine-linux_hotspot_21.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Fri, 01 Dec 2023 07:13:30 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Fri, 01 Dec 2023 07:13:30 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 01 Dec 2023 07:13:31 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 01 Dec 2023 07:13:31 GMT
CMD ["jshell"]
# Tue, 05 Dec 2023 18:31:21 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:31:21 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:31:27 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Tue, 05 Dec 2023 18:31:27 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:31:27 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 05 Dec 2023 18:31:27 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 05 Dec 2023 18:31:27 GMT
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
	-	`sha256:fd0a188ff282b81403d8a726aacd5d985ef4761a8a8f5c876dea381e7a9337a2`  
		Last Modified: Fri, 01 Dec 2023 07:16:52 GMT  
		Size: 157.7 MB (157664998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1103e3032e0ab2751fa60d490107a4b908c287ed9264496a5285c5127ba8a8b1`  
		Last Modified: Fri, 01 Dec 2023 07:16:39 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab03e20f0bc9420a8ab17a6aa1f2cad9ff28b9394902fedb9e44ef361a7edca`  
		Last Modified: Fri, 01 Dec 2023 07:16:39 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9817f09afdf9582e78d44b350f22ea2787f157d0b76a25b2d763dd05cd126c`  
		Last Modified: Tue, 05 Dec 2023 18:42:39 GMT  
		Size: 27.2 MB (27205687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e3c215ca53376fb49edb4e30b1b12cbce2ed6b98a48b64382121cf90ba5e04`  
		Last Modified: Tue, 05 Dec 2023 18:42:37 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8537a105c94db4a4f127dce3b09407ab93a3781da721de72db8ede04f705090c`  
		Last Modified: Tue, 05 Dec 2023 18:42:37 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
