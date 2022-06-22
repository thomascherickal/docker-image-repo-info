## `tomee:9-jre11-alpine-webprofile`

```console
$ docker pull tomee@sha256:0412dd18c7794401af64b9fca3e02d3fab6ac9e60edffaded8397a11acd89666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:9-jre11-alpine-webprofile` - linux; amd64

```console
$ docker pull tomee@sha256:914082a1c4811db96ab998165e4998c34ffa822b397bae38048b9915aef4a692
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107821001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb18208e732e293c5c0a7652b4aec9f1e87f9e5ea05ddafe2ac4346d0c52000f`
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
# Tue, 21 Jun 2022 20:22:14 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Tue, 21 Jun 2022 20:22:45 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='364b0f4faac666a9e81bf17b4e8b5cefa655b0f688cf3e0c1e78eb9d0ce9dca0';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_alpine-linux_hotspot_11.0.15_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 21 Jun 2022 20:22:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Jun 2022 20:22:46 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 21 Jun 2022 21:35:01 GMT
ENV PATH=/usr/local/tomee/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Jun 2022 21:35:01 GMT
RUN mkdir -p /usr/local/tomee
# Tue, 21 Jun 2022 21:35:01 GMT
WORKDIR /usr/local/tomee
# Tue, 21 Jun 2022 21:35:03 GMT
RUN apk add --no-cache gpg gpg-agent dirmngr curl   && rm -rf /var/cache/apk/*
# Tue, 21 Jun 2022 21:35:13 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   B83D15E72253ED1104EB4FBBDAB472F0E5B8A431   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Tue, 21 Jun 2022 21:39:04 GMT
ENV TOMEE_VER=9.0.0-M7
# Tue, 21 Jun 2022 21:39:04 GMT
ENV TOMEE_BUILD=webprofile
# Tue, 21 Jun 2022 21:39:11 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo "`cat tomee.tar.gz.sha512`  apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz" | sha512sum -c   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Tue, 21 Jun 2022 21:39:11 GMT
EXPOSE 8080
# Tue, 21 Jun 2022 21:39:11 GMT
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
	-	`sha256:4e37b5c39ff0662651b864993244fc55c94205e87e616edf9bdb90dc5d93b07a`  
		Last Modified: Tue, 21 Jun 2022 20:27:28 GMT  
		Size: 43.1 MB (43141182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6615a5d94a2abbf699011ec07d6dc79f5903ec4be97abd9e7e9fa9cf85fd55`  
		Last Modified: Tue, 21 Jun 2022 20:27:22 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be178e9415385937b6e14980dcfa448608b9087d90be158391d57ab4824c6ce1`  
		Last Modified: Tue, 21 Jun 2022 22:02:29 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c925adc71e05995499984f010fae83795dd973f9a8c2d325566c7ab820ea1d`  
		Last Modified: Tue, 21 Jun 2022 22:02:30 GMT  
		Size: 6.8 MB (6771626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a84db5356f861d9877af0d8f18e7e57c798a9f3eae83b66cb59b6d50f57770`  
		Last Modified: Tue, 21 Jun 2022 22:02:29 GMT  
		Size: 62.9 KB (62890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6d7b5b27b1fdf7709da0855c435b7e4cab3bb0f448229c6c3e0f004e08ca84`  
		Last Modified: Tue, 21 Jun 2022 22:02:32 GMT  
		Size: 54.6 MB (54568326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
