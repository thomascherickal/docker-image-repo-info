## `clojure:temurin-20-tools-deps-1.11.1.1347-alpine`

```console
$ docker pull clojure@sha256:1d5aa36c35de3a7e5e64f445982dcf94ce3b9ea2a4dfcf3e8fce0009cb18e82c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-20-tools-deps-1.11.1.1347-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:a37c0ebc592be93044b3fb0d4629b2919ec8bed27543272b589c0dab70cdff6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.6 MB (192592245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f8ef042904992c3c6efa1149c629e94d38f0aab54480a175fd6b6132aaa8973`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:11:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 15 Jun 2023 05:11:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 05:11:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Aug 2023 02:38:05 GMT
RUN apk add --no-cache fontconfig java-cacerts libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Thu, 03 Aug 2023 02:38:05 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Thu, 03 Aug 2023 02:38:16 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='b03aced4b7a1c49bc00297e35e45480fd03818862b93e17e1551a3b721e89306';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.2%2B9/OpenJDK20U-jdk_x64_alpine-linux_hotspot_20.0.2_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Thu, 03 Aug 2023 02:38:18 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 03 Aug 2023 02:38:18 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Thu, 03 Aug 2023 02:38:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Aug 2023 02:38:19 GMT
CMD ["jshell"]
# Thu, 03 Aug 2023 05:05:54 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Thu, 03 Aug 2023 05:05:54 GMT
WORKDIR /tmp
# Thu, 03 Aug 2023 05:05:59 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Thu, 03 Aug 2023 05:05:59 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 03 Aug 2023 05:05:59 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 03 Aug 2023 05:05:59 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 03 Aug 2023 05:05:59 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74c4e203881eb96b19b7e16e4d2070742fab18cdfaeb2f07897bd520ec0f868`  
		Last Modified: Thu, 03 Aug 2023 02:42:21 GMT  
		Size: 8.5 MB (8495234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db2f5bca0f22f2f791cbe4b3e7abe717cff049b6dfa83a26912fb609457f068`  
		Last Modified: Thu, 03 Aug 2023 02:42:32 GMT  
		Size: 152.9 MB (152930849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42cb67a7d7a0eb00c40cff496479b26a71b8eb21e657a9f6c644d7a6853e49d7`  
		Last Modified: Thu, 03 Aug 2023 02:42:20 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898b1e6cf835777501f8f1da816adc4f014445b3a3d7f57982b65a6bdc6c2f23`  
		Last Modified: Thu, 03 Aug 2023 02:42:20 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a9a0e67cf068894999137d42bd40d3c93b3283f71e82492d26ed2eaa655a27`  
		Last Modified: Thu, 03 Aug 2023 05:11:14 GMT  
		Size: 27.8 MB (27766410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240d8924ca04839c2594d0b58ab0e93073ea3ac57935979fcabfd2dfd452ebf7`  
		Last Modified: Thu, 03 Aug 2023 05:11:11 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be52742b47ca811fae10bc0ade8e8da37a0f59f0088a6dd2c85ae46ba1a00bb`  
		Last Modified: Thu, 03 Aug 2023 05:11:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
