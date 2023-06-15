## `tomee:8-jre11-Temurin-alpine-webprofile`

```console
$ docker pull tomee@sha256:7e1716f97b9b159a8740ba337c21b81370d51351d03431482bcbcbda8cb519f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre11-Temurin-alpine-webprofile` - linux; amd64

```console
$ docker pull tomee@sha256:6efee8e598e7607759596c785c040e954758cc99534af8a4a016672746c25951
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109741348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55fc9d32bd2769e9db2844ae022ebaa4907979ab54c360dbdef1b784f070df92`
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
# Thu, 15 Jun 2023 05:12:29 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Thu, 15 Jun 2023 05:12:57 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='b5d71cdf3032040e7d2a577712bf525e32e87686af3430219308a39878b98851';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_alpine-linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 15 Jun 2023 05:12:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 15 Jun 2023 08:37:48 GMT
ENV PATH=/usr/local/tomee/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 08:37:48 GMT
RUN mkdir -p /usr/local/tomee ~/.gnupg
# Thu, 15 Jun 2023 08:37:48 GMT
WORKDIR /usr/local/tomee
# Thu, 15 Jun 2023 08:37:50 GMT
RUN apk add --no-cache gpg gpg-agent dirmngr curl   && rm -rf /var/cache/apk/*
# Thu, 15 Jun 2023 08:37:59 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   B83D15E72253ED1104EB4FBBDAB472F0E5B8A431   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 15 Jun 2023 08:37:59 GMT
ENV TOMEE_VER=8.0.15
# Thu, 15 Jun 2023 08:37:59 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 15 Jun 2023 08:38:05 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && sed "s/\t/  /" tomee.tar.gz.sha512 | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 15 Jun 2023 08:38:05 GMT
EXPOSE 8080
# Thu, 15 Jun 2023 08:38:05 GMT
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
	-	`sha256:16832ade66905cf8c5ed94a73a58ea4f631658d206edc31b66059ca91ea645f9`  
		Last Modified: Thu, 15 Jun 2023 05:16:45 GMT  
		Size: 43.1 MB (43129165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244ff747751430c4cd8d4c74a7ba6a2b55e81db6dbf3ff48845e6ac2d6434a46`  
		Last Modified: Thu, 15 Jun 2023 05:16:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1dd2f0f8530bc8e6425ec49825c43469c4565c26b4bd7948cc29ecea575d66`  
		Last Modified: Thu, 15 Jun 2023 08:51:42 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ecd8d22f8b038d85f428712ae8d7c313fd7e1b936db3170507a57fcbf098b`  
		Last Modified: Thu, 15 Jun 2023 08:51:43 GMT  
		Size: 6.5 MB (6549110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa884ba5821e8a1901a0a0d373805a8bdb65a4792101b9891614e447aa1e2b8d`  
		Last Modified: Thu, 15 Jun 2023 08:51:42 GMT  
		Size: 62.9 KB (62932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e32cb2961a27a501cad3137171244a741e9df8dd5e0860ba1e386c80ac4ce4`  
		Last Modified: Thu, 15 Jun 2023 08:51:45 GMT  
		Size: 49.0 MB (48953509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
