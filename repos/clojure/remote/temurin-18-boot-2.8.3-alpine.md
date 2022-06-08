## `clojure:temurin-18-boot-2.8.3-alpine`

```console
$ docker pull clojure@sha256:7d93106f983834b45afa42b13c0ea2634b8c989e5161d3445b7fe03322b451d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-18-boot-2.8.3-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:b994ae41322de1daa52c4a70f044be0baa4ce60532d538384f836e142527d3e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.8 MB (255778569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b353743839d4be682be1dbb11e2724a678ac4d1fbc2cdb67f47055d603c34744`
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
# Wed, 08 Jun 2022 19:05:05 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 08 Jun 2022 19:05:05 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 08 Jun 2022 19:05:05 GMT
WORKDIR /tmp
# Wed, 08 Jun 2022 19:05:07 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Wed, 08 Jun 2022 19:05:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 08 Jun 2022 19:05:07 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 08 Jun 2022 19:05:43 GMT
RUN boot
# Wed, 08 Jun 2022 19:05:43 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 08 Jun 2022 19:05:44 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 08 Jun 2022 19:05:44 GMT
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
	-	`sha256:a4999eef7250c59af1e8ce612900661002c5085eced42d5c29d3c1d0aa438775`  
		Last Modified: Wed, 08 Jun 2022 18:27:39 GMT  
		Size: 192.9 MB (192862537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262edfdf635ac957aea206f1847f59984d074da776116ffbfaadedb1b331f18b`  
		Last Modified: Wed, 08 Jun 2022 18:27:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8f6b9308cd489a5e2cc472b3e82d546254f3269a5818a470a28ceac1d4ad80`  
		Last Modified: Wed, 08 Jun 2022 19:09:11 GMT  
		Size: 849.6 KB (849624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a12aa80efeb77e952c69a2a5d5a6f1ddb8ff3d8b9693862dc1a6313034b6441`  
		Last Modified: Wed, 08 Jun 2022 19:09:20 GMT  
		Size: 58.8 MB (58820841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a38f1e97e262446fc1351b8c6f3e4198eeef9906538e18986dff72f85d79238`  
		Last Modified: Wed, 08 Jun 2022 19:09:11 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
