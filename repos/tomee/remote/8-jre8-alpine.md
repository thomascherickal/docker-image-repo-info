## `tomee:8-jre8-alpine`

```console
$ docker pull tomee@sha256:d4bf5689ce0126c3a02d7e8e2bacdde5901bb4f9fdc79eecadef9c3badf5ee82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre8-alpine` - linux; amd64

```console
$ docker pull tomee@sha256:f68c3f1e17d8a6366d3e6884838426e634e064408b1b94ff76bfbdf3bf824eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.4 MB (108387845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9371483291faab2ca3a8c4125ef5fc15cc6d8d7c9c9d3434294aa1dbb6d763`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 24 May 2023 23:34:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 24 May 2023 23:34:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 May 2023 23:34:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 24 May 2023 23:34:29 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Wed, 24 May 2023 23:34:29 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 24 May 2023 23:34:50 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='95d8cb8b5375ec00a064ed728eb60d925d44c1a79fe92f6ca7385b5863d4f78c';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_alpine-linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 24 May 2023 23:34:50 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 26 May 2023 00:34:01 GMT
ENV PATH=/usr/local/tomee/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jun 2023 20:31:50 GMT
RUN mkdir -p /usr/local/tomee ~/.gnupg
# Thu, 08 Jun 2023 20:31:50 GMT
WORKDIR /usr/local/tomee
# Thu, 08 Jun 2023 20:31:52 GMT
RUN apk add --no-cache gpg gpg-agent dirmngr curl   && rm -rf /var/cache/apk/*
# Thu, 08 Jun 2023 20:32:01 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   B83D15E72253ED1104EB4FBBDAB472F0E5B8A431   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 08 Jun 2023 20:32:01 GMT
ENV TOMEE_VER=8.0.15
# Thu, 08 Jun 2023 20:32:01 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 08 Jun 2023 20:32:07 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && sed "s/\t/  /" tomee.tar.gz.sha512 | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 08 Jun 2023 20:32:07 GMT
EXPOSE 8080
# Thu, 08 Jun 2023 20:32:07 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdde4a302e0d0ee2ef6760bf84344d762835ef2d38d2a1a1062c7d038fe2615b`  
		Last Modified: Wed, 24 May 2023 23:37:36 GMT  
		Size: 7.6 MB (7648427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf96ab42c6c4994c00287d16df6cf42f90d380ef00732e97e569b1a39d56d273`  
		Last Modified: Wed, 24 May 2023 23:37:58 GMT  
		Size: 41.8 MB (41776015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5a9287dcf663188b76b1a9b04971a29e183fe0764a683c005bdc5f7c54418a`  
		Last Modified: Wed, 24 May 2023 23:37:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d92a7fb3b8fc8acda76338d3b98a20d25deabd64b75b52f8202e7d3f686e645`  
		Last Modified: Thu, 08 Jun 2023 21:04:06 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d637fe181dc2471a7b143eb0ceb1f855fe8b291c70ed92573ecf2d4c6eefb458`  
		Last Modified: Thu, 08 Jun 2023 21:04:07 GMT  
		Size: 6.5 MB (6549122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a450a1b1c10a80de86a532011c798d6dcd5c1b28839475cf474b0267ed7321d2`  
		Last Modified: Thu, 08 Jun 2023 21:04:06 GMT  
		Size: 62.9 KB (62943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e859a64c5153e95edea2b33c020a49c75611ae1dcb70152703380ba491d9482`  
		Last Modified: Thu, 08 Jun 2023 21:04:09 GMT  
		Size: 49.0 MB (48953467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
