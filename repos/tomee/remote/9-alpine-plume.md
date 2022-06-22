## `tomee:9-alpine-plume`

```console
$ docker pull tomee@sha256:8fab0481774109f228d77ce02fa1809cb14982e7e012b65f8493dce5969ff08c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:9-alpine-plume` - linux; amd64

```console
$ docker pull tomee@sha256:f25829874a9628c7a552100dc82b44555e1febf5b3783a251cf98f4d0e55905b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135175463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8366a1d265b0d225fe870dc3354ac6648b331aa2574f12df5e387b6445277708`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 21 Jun 2022 20:21:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 21 Jun 2022 20:21:36 GMT
RUN apk add --no-cache libretls musl-locales musl-locales-lang tzdata zlib     && rm -rf /var/cache/apk/*
# Tue, 21 Jun 2022 20:22:54 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Tue, 21 Jun 2022 20:23:33 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='27e4589db9b8e6df60a75737f12ab7df63f796ecf8e46c0a196f77b2c99af1ac';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_alpine-linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 21 Jun 2022 20:23:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Jun 2022 20:23:34 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 21 Jun 2022 21:33:40 GMT
ENV PATH=/usr/local/tomee/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Jun 2022 21:33:40 GMT
RUN mkdir -p /usr/local/tomee
# Tue, 21 Jun 2022 21:33:40 GMT
WORKDIR /usr/local/tomee
# Tue, 21 Jun 2022 21:34:20 GMT
RUN apk add --no-cache gpg gpg-agent dirmngr curl  && rm -rf /var/cache/apk/*
# Tue, 21 Jun 2022 21:34:29 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   B83D15E72253ED1104EB4FBBDAB472F0E5B8A431   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Tue, 21 Jun 2022 21:38:23 GMT
ENV TOMEE_VER=9.0.0-M7
# Tue, 21 Jun 2022 21:38:23 GMT
ENV TOMEE_BUILD=plume
# Tue, 21 Jun 2022 21:38:32 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo "`cat tomee.tar.gz.sha512`  apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz" | sha512sum -c   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Tue, 21 Jun 2022 21:38:32 GMT
EXPOSE 8080
# Tue, 21 Jun 2022 21:38:32 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4177d2591259bff2bae6f43f12721dbe4ed5aac24fb0991377a3d27cdd534e`  
		Last Modified: Tue, 21 Jun 2022 20:26:07 GMT  
		Size: 477.8 KB (477755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26871a4cf158323669bba53c8eb06b2dbf45ee4d605808080f05c0711812a52a`  
		Last Modified: Tue, 21 Jun 2022 20:28:17 GMT  
		Size: 46.6 MB (46582111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e16f89265d6405d62f4f956e52070c45c8e2546c67fe8e5d2abe1c16411e46`  
		Last Modified: Tue, 21 Jun 2022 20:28:10 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3795810670d115bc1cde940c145276e20fa6d1764d6d0943a8b59152dbd69d`  
		Last Modified: Tue, 21 Jun 2022 21:58:05 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec6e174b21ddb764cd7eabeed897b009af1d6337e70b53f15d7ef12c4429cf3`  
		Last Modified: Tue, 21 Jun 2022 22:00:31 GMT  
		Size: 6.8 MB (6771622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036896af0268732b542ae4ed52816a15370b7b3238abcb83f2af38e924916947`  
		Last Modified: Tue, 21 Jun 2022 22:00:30 GMT  
		Size: 62.9 KB (62906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087c77d330726f1845edabb4c5986f82f8f0b683d6b43e280dc586221faef281`  
		Last Modified: Tue, 21 Jun 2022 22:00:34 GMT  
		Size: 78.5 MB (78481847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
