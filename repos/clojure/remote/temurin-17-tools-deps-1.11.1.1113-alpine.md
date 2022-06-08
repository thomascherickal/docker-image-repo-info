## `clojure:temurin-17-tools-deps-1.11.1.1113-alpine`

```console
$ docker pull clojure@sha256:0aed5054fa5e5cee4b6ceb1b8f11689167a06e2dbaa59679d92e356cd2c0f241
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-17-tools-deps-1.11.1.1113-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:b61a4c4801796bbd7cf9ec5ec9e3a932483b588a4782938cb250466c3e0a8be2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.2 MB (225176393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b4dcf309df8a6b53ac513a70cf84b24bf394d7bfe8bbbc2faedf6c512b5f7c5`
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
# Wed, 08 Jun 2022 18:22:03 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Wed, 08 Jun 2022 18:22:17 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='5cbaece6aec44f6d3911cfa3c5a8659889e85042aff214c944c5fa1b5938a5fc';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 08 Jun 2022 18:22:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Jun 2022 18:22:19 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 08 Jun 2022 18:22:19 GMT
CMD ["jshell"]
# Wed, 08 Jun 2022 19:04:53 GMT
ENV CLOJURE_VERSION=1.11.1.1113
# Wed, 08 Jun 2022 19:04:53 GMT
WORKDIR /tmp
# Wed, 08 Jun 2022 19:04:59 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "7677bb1179ebb15ebf954a87bd1078f1c547673d946dadafd23ece8cd61f5a9f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Wed, 08 Jun 2022 19:04:59 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 08 Jun 2022 19:04:59 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 08 Jun 2022 19:04:59 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 08 Jun 2022 19:04:59 GMT
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
	-	`sha256:5b675003cef6d41754d8984fa5998377cd14cb310f6d34d51d3105e9572af398`  
		Last Modified: Wed, 08 Jun 2022 18:26:48 GMT  
		Size: 191.8 MB (191809203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29402433809ae92da2b8604813d0a262eff1bdf9a6d1120c927de504e14e1a`  
		Last Modified: Wed, 08 Jun 2022 18:26:33 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb18b22a4dbc1d7ee12fc6ee870fed458b802c1b22c5197ab39d670d07ce4d`  
		Last Modified: Wed, 08 Jun 2022 19:08:53 GMT  
		Size: 30.1 MB (30120999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd6a6423c66d91d3e5a25f46ff7cc8854bb1f00794a4961f55e358963d995b3`  
		Last Modified: Wed, 08 Jun 2022 19:08:50 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6608a815d17e57cdbd1884148d4236cd1ebf60332da6e83bf9909a96123a31`  
		Last Modified: Wed, 08 Jun 2022 19:08:50 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
