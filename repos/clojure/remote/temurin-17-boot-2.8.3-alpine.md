## `clojure:temurin-17-boot-2.8.3-alpine`

```console
$ docker pull clojure@sha256:493dbcd306e668be729e0cf8b0890b2bdc24702a6a425ae15264edfbdbef5a61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-17-boot-2.8.3-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:4477fcb95e0e50087c9747500966636fd623ec70b48337951a498d6c18e10a3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254725758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c701eb763cae3864d5bd0861745700f1e7f59965916116ece227e923235467e5`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

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
# Wed, 08 Jun 2022 19:02:53 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 08 Jun 2022 19:02:53 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 08 Jun 2022 19:02:53 GMT
WORKDIR /tmp
# Wed, 08 Jun 2022 19:02:56 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Wed, 08 Jun 2022 19:02:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 08 Jun 2022 19:02:56 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 08 Jun 2022 19:04:16 GMT
RUN boot
# Wed, 08 Jun 2022 19:04:17 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 08 Jun 2022 19:04:17 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 08 Jun 2022 19:04:17 GMT
CMD ["repl"]
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
	-	`sha256:fb6e25f999f90987f115b60c6d5189654df65d5714e095ba5d02d2b804cd9a70`  
		Last Modified: Wed, 08 Jun 2022 19:08:16 GMT  
		Size: 849.6 KB (849616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42aff64fe0daea1a3bb8b4c543ff8dd67fc39e63d5f75c288673622c6eb3025`  
		Last Modified: Wed, 08 Jun 2022 19:08:19 GMT  
		Size: 58.8 MB (58821374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f330f8e4458b9b2ea0b480e17e1eee6cd1d6365f8e6dc58782dd6025d65135`  
		Last Modified: Wed, 08 Jun 2022 19:08:15 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
