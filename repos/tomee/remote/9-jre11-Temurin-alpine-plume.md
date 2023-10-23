## `tomee:9-jre11-Temurin-alpine-plume`

```console
$ docker pull tomee@sha256:13d8a6dae8eb066a1a1b24116f1bcabc1070d9c4868d5d79b9dd631a4d4af319
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:9-jre11-Temurin-alpine-plume` - linux; amd64

```console
$ docker pull tomee@sha256:233668afc0d056abf309a3edb70204472a168137f4ddbc472e50da3b218ed121
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.6 MB (143574772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01bc10e0c6697bd6701edac41efecc0fa985cc0be7aa68c56a876a4bcf1676b4`
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
# Thu, 19 Oct 2023 02:51:15 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Thu, 19 Oct 2023 02:51:55 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d34ea3d1e3852548546c69d7d73addb873e7926e66147b8596b7c11fad9ee057';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_x64_alpine-linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Thu, 19 Oct 2023 02:51:56 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 19 Oct 2023 02:51:56 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Thu, 19 Oct 2023 02:51:56 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Thu, 19 Oct 2023 08:06:59 GMT
ENV PATH=/usr/local/tomee/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Oct 2023 08:06:59 GMT
RUN mkdir -p /usr/local/tomee ~/.gnupg
# Thu, 19 Oct 2023 08:06:59 GMT
WORKDIR /usr/local/tomee
# Thu, 19 Oct 2023 08:07:31 GMT
RUN apk add --no-cache gpg gpg-agent dirmngr curl  && rm -rf /var/cache/apk/*
# Thu, 19 Oct 2023 08:07:39 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   B83D15E72253ED1104EB4FBBDAB472F0E5B8A431   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Mon, 23 Oct 2023 22:27:46 GMT
ENV TOMEE_VER=9.1.1
# Mon, 23 Oct 2023 22:27:46 GMT
ENV TOMEE_BUILD=plume
# Mon, 23 Oct 2023 22:27:55 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && sed "s/\t/  /" tomee.tar.gz.sha512 | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Mon, 23 Oct 2023 22:27:55 GMT
EXPOSE 8080
# Mon, 23 Oct 2023 22:27:55 GMT
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
	-	`sha256:26fdf8e4c3c8b44c87504ef46a614d2ba962bb2d09033777bffab7c71b8f1a11`  
		Last Modified: Thu, 19 Oct 2023 02:57:36 GMT  
		Size: 43.3 MB (43296812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9e2b841b36766636846f36938958fdd21f69e97de85a5879412582425e43b9`  
		Last Modified: Thu, 19 Oct 2023 02:57:31 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8468eb18380472ab706014090430b501e0ebfbede999a572ceb1521dede2eae`  
		Last Modified: Thu, 19 Oct 2023 02:57:31 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22751a1865e07e04f7f1f02ca0227af79107ee4f41d9581f484c2b750126807b`  
		Last Modified: Thu, 19 Oct 2023 08:22:07 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fd11e16301872b4ed43743efffc6fb44d3358467d5189cb8a33307671e1614`  
		Last Modified: Thu, 19 Oct 2023 08:23:17 GMT  
		Size: 5.8 MB (5789805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8246e7b5199dfadbfb1d14e3673240ac4cca3efcb59e3cdc10e7aaf75d047a2d`  
		Last Modified: Thu, 19 Oct 2023 08:23:16 GMT  
		Size: 62.9 KB (62933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a383fffd0e86a0735778d4a78d7ed84ac6ec58f1b734de003159cb18e2dc894`  
		Last Modified: Mon, 23 Oct 2023 22:51:36 GMT  
		Size: 81.7 MB (81745654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
