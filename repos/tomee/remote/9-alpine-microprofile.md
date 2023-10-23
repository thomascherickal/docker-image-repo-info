## `tomee:9-alpine-microprofile`

```console
$ docker pull tomee@sha256:b4beaf3aebbdba60ea6ebf45c4ac537bed8acbb4e050738a03676edba37acb0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:9-alpine-microprofile` - linux; amd64

```console
$ docker pull tomee@sha256:545090f86816c24be8f6a1c994d2dac83a24e78047507e182c4ff48f9a0cbf22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134120839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42879cd761deaca06baabc73162b410dbf619a3567ed73af3bc94ac9a6d4a6fd`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 02:50:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 19 Oct 2023 02:50:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Oct 2023 02:50:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 19 Oct 2023 02:50:17 GMT
RUN apk add --no-cache fontconfig java-cacerts bash libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Thu, 19 Oct 2023 02:52:13 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Thu, 19 Oct 2023 02:52:53 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bf726bb99785901f22849a0ef4ddd4e67f3e5b184dbbf260fffbaf5befce18a3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jre_x64_alpine-linux_hotspot_17.0.8.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Thu, 19 Oct 2023 02:52:53 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 19 Oct 2023 02:52:54 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Thu, 19 Oct 2023 02:52:54 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Thu, 19 Oct 2023 08:05:28 GMT
ENV PATH=/usr/local/tomee/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Oct 2023 08:05:29 GMT
RUN mkdir -p /usr/local/tomee ~/.gnupg
# Thu, 19 Oct 2023 08:05:29 GMT
WORKDIR /usr/local/tomee
# Thu, 19 Oct 2023 08:05:50 GMT
RUN apk add --no-cache gpg gpg-agent gpg-agent dirmngr curl   && rm -rf /var/cache/apk/*
# Thu, 19 Oct 2023 08:05:59 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   B83D15E72253ED1104EB4FBBDAB472F0E5B8A431   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Mon, 23 Oct 2023 22:26:02 GMT
ENV TOMEE_VER=9.1.1
# Mon, 23 Oct 2023 22:26:02 GMT
ENV TOMEE_BUILD=microprofile
# Mon, 23 Oct 2023 22:26:10 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && sed "s/\t/  /" tomee.tar.gz.sha512 | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Mon, 23 Oct 2023 22:26:10 GMT
EXPOSE 8080
# Mon, 23 Oct 2023 22:26:10 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42efc8ffaa989c4197765e315c7d229fc40528c139b6be6a50e459fab1b640e`  
		Last Modified: Thu, 19 Oct 2023 02:55:23 GMT  
		Size: 9.3 MB (9276490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcde25b0c532a5736d3be02fdc2c5f1c87fec5df1dba88a208d4949591d871d6`  
		Last Modified: Thu, 19 Oct 2023 02:59:00 GMT  
		Size: 47.0 MB (46964309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec0ff88a394946ae5b6d16bb310a372fc7269f1c63d24092408b744039db4d4`  
		Last Modified: Thu, 19 Oct 2023 02:58:53 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea012f7c346eb412866da9f6f36bd0859cd146d768884691aae00fe2d37fe783`  
		Last Modified: Thu, 19 Oct 2023 02:58:53 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444784a132a7663ccb307eade8b0b366d1cb016454ab2e3605afc6684dc9dec0`  
		Last Modified: Thu, 19 Oct 2023 08:18:04 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bea894cf6d36f82cc24bc06b921ea29fc94658b2c17e80e14e5018dc96bedd9`  
		Last Modified: Thu, 19 Oct 2023 08:19:27 GMT  
		Size: 5.8 MB (5789809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40592786b6f731f78d8be482e3ed9f075f2ebf5ebd7f74a333170ecac1745c2`  
		Last Modified: Thu, 19 Oct 2023 08:19:26 GMT  
		Size: 62.9 KB (62943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f6e19b6e45eea4a6f9f50044ac07345df090c16301ba82ec76727da72a4d62`  
		Last Modified: Mon, 23 Oct 2023 22:45:50 GMT  
		Size: 68.6 MB (68624214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
