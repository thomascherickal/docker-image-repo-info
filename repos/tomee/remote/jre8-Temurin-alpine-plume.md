## `tomee:jre8-Temurin-alpine-plume`

```console
$ docker pull tomee@sha256:0628187a6f290215b1006bef32b6541e5c85d3be5e53caceaba7e5cc2b81fcf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:jre8-Temurin-alpine-plume` - linux; amd64

```console
$ docker pull tomee@sha256:68a310d7f1c1dafb70c802d9e5fd3c9ad9741794b8075b57e20fc7f598ef9481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138069509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ae7cc0f48c91f3a1a291240055a45045b3bce642b46223c7b7c9884a011d3d`
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
# Thu, 19 Oct 2023 02:50:17 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Thu, 19 Oct 2023 02:50:58 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7040d865493f13204194c5a1add63e22516b1fa4481264baa6a5b2614a275a0e';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_alpine-linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Thu, 19 Oct 2023 02:50:58 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 19 Oct 2023 02:50:59 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Thu, 19 Oct 2023 02:50:59 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Thu, 19 Oct 2023 08:08:13 GMT
ENV PATH=/usr/local/tomee/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Oct 2023 08:08:14 GMT
RUN mkdir -p /usr/local/tomee ~/.gnupg
# Thu, 19 Oct 2023 08:08:14 GMT
WORKDIR /usr/local/tomee
# Thu, 19 Oct 2023 08:08:46 GMT
RUN apk add --no-cache gpg gpg-agent dirmngr curl  && rm -rf /var/cache/apk/*
# Thu, 19 Oct 2023 08:08:54 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   B83D15E72253ED1104EB4FBBDAB472F0E5B8A431   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 19 Oct 2023 08:08:54 GMT
ENV TOMEE_VER=8.0.15
# Thu, 19 Oct 2023 08:08:54 GMT
ENV TOMEE_BUILD=plume
# Thu, 19 Oct 2023 08:09:02 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && sed "s/\t/  /" tomee.tar.gz.sha512 | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 19 Oct 2023 08:09:03 GMT
EXPOSE 8080
# Thu, 19 Oct 2023 08:09:03 GMT
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
	-	`sha256:e905b36c06d1b3c68af07bdee9b26c29801e70572bcb79978b3216828ad8bc15`  
		Last Modified: Thu, 19 Oct 2023 02:56:14 GMT  
		Size: 41.8 MB (41790480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1767ee2c762b19697307d41a746a2206da6b8f4771db2740abfe160f921da992`  
		Last Modified: Thu, 19 Oct 2023 02:56:07 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb038c37b8688e76e5e2a758e0f6e575b3f6a2d75277e212231d728a538360`  
		Last Modified: Thu, 19 Oct 2023 02:56:07 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61604dce47f6c07d04996e54a143b6e6a1c868dc15ee475f4c06e1384641d9a`  
		Last Modified: Thu, 19 Oct 2023 08:24:39 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b5813874f1343735934318de4f6733fc2d846bbfcf94ef74da74cfbf05b3bc`  
		Last Modified: Thu, 19 Oct 2023 08:25:48 GMT  
		Size: 5.8 MB (5789798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4651afd5b20b3a7600bd642b5d8ca736f982aab216c9a8e6f26466896e0bec9f`  
		Last Modified: Thu, 19 Oct 2023 08:25:48 GMT  
		Size: 62.9 KB (62932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11dc498af30838b56c3258f6cf0fd4846e0b6261fb646539119675deb1f14d67`  
		Last Modified: Thu, 19 Oct 2023 08:25:53 GMT  
		Size: 77.7 MB (77746733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
