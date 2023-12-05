## `clojure:temurin-8-alpine`

```console
$ docker pull clojure@sha256:1150722445e7e4bd4e24e52607ab4f0313ac10b0f0a83a3ccbc09bd52918ef03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-8-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:d78251e406d12dfb2f488ab376ef9e2ceb0ce9c1469596d44c5cc9fc0be1178b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141390471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db41149dda49041c94f3c70e659f628604e5692f4c02606cb809e1064fcf04b`
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
# Fri, 01 Dec 2023 07:11:20 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Fri, 01 Dec 2023 07:11:26 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='8dcb1532a1194afa06e4b5ace4e9e279926392442bf46b2d51b49ae1a9a1dfea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_alpine-linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Fri, 01 Dec 2023 07:11:27 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Fri, 01 Dec 2023 07:11:27 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 01 Dec 2023 07:11:27 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 05 Dec 2023 18:22:28 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:22:28 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:22:34 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Tue, 05 Dec 2023 18:22:34 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:22:34 GMT
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
	-	`sha256:732fa2d489935267fd2bbf96196e8455c977d24cc2c9d81f2ee3219e8418975c`  
		Last Modified: Fri, 01 Dec 2023 07:14:48 GMT  
		Size: 101.5 MB (101507632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434ffde56a8199b544e2f12cacdf53f51218e13142b5ae4c7bdade14b874feb2`  
		Last Modified: Fri, 01 Dec 2023 07:14:39 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2a63ca63e4b1113d3add2880bff63c7c0c55d2bf156dba4057b899357832cb`  
		Last Modified: Fri, 01 Dec 2023 07:14:40 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341b63aa86bbc0f9f296149958f9c0c7b925049497cab98c752c73ebe75dfd62`  
		Last Modified: Tue, 05 Dec 2023 18:35:41 GMT  
		Size: 27.2 MB (27202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a73cc30ddd2809e085919b6b114e06d2a0e446bba5a3c1e06353ecf647bc25`  
		Last Modified: Tue, 05 Dec 2023 18:35:39 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
