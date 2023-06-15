## `tomee:8-Temurin-alpine-plume`

```console
$ docker pull tomee@sha256:c3c51f9c0c0a50e0ce248b05c8d95c08e8831736a815fa1072a0cc385fc8a8f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-Temurin-alpine-plume` - linux; amd64

```console
$ docker pull tomee@sha256:87491438326d57f717429befea0e7c308f924694ece8db816e28b0f466f8e44c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142181978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b8fc37a3b393b96d911c102ff151b11cfec22de944319a41698c32e6b280971`
-	Default Command: `["catalina.sh","run"]`

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
# Thu, 15 Jun 2023 05:11:54 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Thu, 15 Jun 2023 05:13:09 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Thu, 15 Jun 2023 05:13:39 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='711f837bacf8222dee9e8cd7f39941a4a0acf869243f03e6038ca3ba189f66ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_alpine-linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 15 Jun 2023 05:13:40 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 15 Jun 2023 08:36:24 GMT
ENV PATH=/usr/local/tomee/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 08:36:24 GMT
RUN mkdir -p /usr/local/tomee ~/.gnupg
# Thu, 15 Jun 2023 08:36:24 GMT
WORKDIR /usr/local/tomee
# Thu, 15 Jun 2023 08:37:06 GMT
RUN apk add --no-cache gpg gpg-agent dirmngr curl  && rm -rf /var/cache/apk/*
# Thu, 15 Jun 2023 08:37:15 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   B83D15E72253ED1104EB4FBBDAB472F0E5B8A431   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 15 Jun 2023 08:37:15 GMT
ENV TOMEE_VER=8.0.15
# Thu, 15 Jun 2023 08:37:15 GMT
ENV TOMEE_BUILD=plume
# Thu, 15 Jun 2023 08:37:22 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && sed "s/\t/  /" tomee.tar.gz.sha512 | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 15 Jun 2023 08:37:23 GMT
EXPOSE 8080
# Thu, 15 Jun 2023 08:37:23 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aadc9aaa732ac5b0edd00545607971071fa1868047a65249e483ba2443982e6`  
		Last Modified: Thu, 15 Jun 2023 05:15:34 GMT  
		Size: 7.6 MB (7648372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f065ea542023b30d5a52e2ccef4e2db263aaec4fac56317ebed73d525ed11e`  
		Last Modified: Thu, 15 Jun 2023 05:17:32 GMT  
		Size: 46.8 MB (46776655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff25c436cb1413e375f1fad11f51fc222b8313015736df4ef8f5842f3db19fcd`  
		Last Modified: Thu, 15 Jun 2023 05:17:26 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ce1c83ae88c885f1faabcc490cc3925496dbeb50816d1d85049f977e7157a3`  
		Last Modified: Thu, 15 Jun 2023 08:48:15 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115eb7ef1d6bc9584eb0aeebc3adb933303b26af5538e787e4b8cb0946946f9c`  
		Last Modified: Thu, 15 Jun 2023 08:50:01 GMT  
		Size: 6.5 MB (6549020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f210cecabb683bb362b5c070a8aa3a0996a4137b7411e07496e579cee2d3c644`  
		Last Modified: Thu, 15 Jun 2023 08:50:00 GMT  
		Size: 63.0 KB (62957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a0d3e06f741ca9b0af62fb4841a741bb370486d18faccdeb54de535d3dd308`  
		Last Modified: Thu, 15 Jun 2023 08:50:04 GMT  
		Size: 77.7 MB (77746716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
