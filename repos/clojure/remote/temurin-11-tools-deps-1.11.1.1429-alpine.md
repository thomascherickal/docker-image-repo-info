## `clojure:temurin-11-tools-deps-1.11.1.1429-alpine`

```console
$ docker pull clojure@sha256:3fdbf720f3076b17f5b0debc7a394b186c0f71cab88d9bf10ddd68759cc02489
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-11-tools-deps-1.11.1.1429-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:5387bc32df50cff0c4c1dad69f5fae9fb0d5bc22d9b33717838aced8cd10e2d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.4 MB (180367479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d70b60a5442cff4fd676dd18df5ada88e1db6b6b279523c5a2d010d696775c`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["clj"]`

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
# Fri, 01 Dec 2023 07:11:20 GMT
RUN set -eux;     apk add --no-cache         bash         fontconfig ttf-dejavu         java-cacerts         libretls zlib         musl-locales musl-locales-lang         tzdata     ;     rm -rf /var/cache/apk/*
# Fri, 01 Dec 2023 07:11:56 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Fri, 01 Dec 2023 07:12:05 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d5e2235d3707526f7c9ba3f0dc194e60d5dec33eceff2a2dcf9d874464cc0e9e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Fri, 01 Dec 2023 07:12:07 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Fri, 01 Dec 2023 07:12:07 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 01 Dec 2023 07:12:07 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 01 Dec 2023 07:12:08 GMT
CMD ["jshell"]
# Tue, 05 Dec 2023 18:25:52 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:25:52 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:25:57 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Tue, 05 Dec 2023 18:25:57 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:25:57 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ce2a3866efc31d675066df134952e4237faaf14332528051e5efca30a21a4a`  
		Last Modified: Fri, 01 Dec 2023 07:14:41 GMT  
		Size: 9.3 MB (9276515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629c7d34e934cd201a8e75a722510b7ee2941ad0e9fa3f00aad45123b459e506`  
		Last Modified: Fri, 01 Dec 2023 07:15:27 GMT  
		Size: 140.5 MB (140484666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32732554e58223c82fef201a71a8024d58729978033c9b6c7c8f21f0dbe8c4`  
		Last Modified: Fri, 01 Dec 2023 07:15:17 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ff009245964d87749ff002f164205f495cf779e600805d759bcbb573dfb22f`  
		Last Modified: Fri, 01 Dec 2023 07:15:17 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b0500db91a9bcc078c20984b61a58e50789b0da59d05e9021d149c77a5a4b6`  
		Last Modified: Tue, 05 Dec 2023 18:37:59 GMT  
		Size: 27.2 MB (27202344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2061e88e99c644c2cfb54dc50016aa44b614f8faff65c5641d5d682403ea39b3`  
		Last Modified: Tue, 05 Dec 2023 18:37:56 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
