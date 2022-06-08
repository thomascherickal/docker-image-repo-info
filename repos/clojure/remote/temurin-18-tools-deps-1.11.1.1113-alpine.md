## `clojure:temurin-18-tools-deps-1.11.1.1113-alpine`

```console
$ docker pull clojure@sha256:245d24ab50c4b4c2aec33aaec8e3a527913d2361842db062138f010b917417f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-18-tools-deps-1.11.1.1113-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:1725a877e158bfdb012431cc170588a2756a3b68cad808b14991861c8693fab8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.2 MB (226229680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152ac8a2a6f285efbd973c203e8928e432d818107d5b46823f77891a43b85567`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:55:43 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 08 Jun 2022 18:20:30 GMT
RUN apk add --no-cache libretls musl-locales musl-locales-lang tzdata zlib     && rm -rf /var/cache/apk/*
# Wed, 08 Jun 2022 18:22:46 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 08 Jun 2022 18:23:06 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ab72b28e1ce896e6b11e2b362c12c36007ebe9963d8954bc11e637be1f024dfe';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_alpine-linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 08 Jun 2022 18:23:06 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Jun 2022 18:23:07 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 08 Jun 2022 18:23:07 GMT
CMD ["jshell"]
# Wed, 08 Jun 2022 19:06:11 GMT
ENV CLOJURE_VERSION=1.11.1.1113
# Wed, 08 Jun 2022 19:06:11 GMT
WORKDIR /tmp
# Wed, 08 Jun 2022 19:06:16 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "7677bb1179ebb15ebf954a87bd1078f1c547673d946dadafd23ece8cd61f5a9f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Wed, 08 Jun 2022 19:06:16 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 08 Jun 2022 19:06:16 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 08 Jun 2022 19:06:17 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 08 Jun 2022 19:06:17 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611b459a9f120c9f22143fbef6dda47c621957b1c86d4cbdf8fe3d9c762d728`  
		Last Modified: Wed, 08 Jun 2022 18:25:04 GMT  
		Size: 430.4 KB (430445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4999eef7250c59af1e8ce612900661002c5085eced42d5c29d3c1d0aa438775`  
		Last Modified: Wed, 08 Jun 2022 18:27:39 GMT  
		Size: 192.9 MB (192862537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262edfdf635ac957aea206f1847f59984d074da776116ffbfaadedb1b331f18b`  
		Last Modified: Wed, 08 Jun 2022 18:27:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b58c4aeeae62f87fbbba498f8215fccad958b0dbd4e30a3cdce09d36115fce1`  
		Last Modified: Wed, 08 Jun 2022 19:09:48 GMT  
		Size: 30.1 MB (30120948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52392e47568476cfb9b8fa1024274d5469c73ee5b5c94c06c9cf1e436889ae4f`  
		Last Modified: Wed, 08 Jun 2022 19:09:45 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50acd0b28bc090d34616e95856de5cdba9f9b921ceeb39760dd5bbfbacb1366`  
		Last Modified: Wed, 08 Jun 2022 19:09:45 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
