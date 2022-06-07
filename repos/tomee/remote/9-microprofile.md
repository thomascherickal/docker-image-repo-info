## `tomee:9-microprofile`

```console
$ docker pull tomee@sha256:533cdca11e707a4251915e7368ed2f8179b4f783b2d909788a08e605b09bda52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomee:9-microprofile` - linux; amd64

```console
$ docker pull tomee@sha256:948bd7b5d4399cbd57e81bace00ce7b9c313949b6e06f71a973b2c9a12c4c886
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164518613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87ba0ea302c8b3c25b74ed96107113fb94dfed6774bcd7e3eed11cc1828e59e7`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:12:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 00:15:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:15:30 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Tue, 07 Jun 2022 00:16:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 00:16:22 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 00:16:22 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 07 Jun 2022 05:10:16 GMT
ENV PATH=/usr/local/tomee/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 05:10:16 GMT
RUN mkdir -p /usr/local/tomee
# Tue, 07 Jun 2022 05:10:16 GMT
WORKDIR /usr/local/tomee
# Tue, 07 Jun 2022 05:10:24 GMT
RUN apt-get update   && apt-get install -y  gpg   && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:10:34 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   B83D15E72253ED1104EB4FBBDAB472F0E5B8A431   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Tue, 07 Jun 2022 05:16:37 GMT
ENV TOMEE_VER=9.0.0-M7
# Tue, 07 Jun 2022 05:16:55 GMT
ENV TOMEE_BUILD=microprofile
# Tue, 07 Jun 2022 05:17:02 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Tue, 07 Jun 2022 05:17:02 GMT
EXPOSE 8080
# Tue, 07 Jun 2022 05:17:02 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32598539a8f0b55be77078c6637866fc4128a4213ea59e9993662a310a2b711`  
		Last Modified: Tue, 07 Jun 2022 00:22:05 GMT  
		Size: 19.8 MB (19773881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c96f165def119d706c2e86c082214c93a07343edb524cc95a4c7701447e5f3d`  
		Last Modified: Tue, 07 Jun 2022 00:23:04 GMT  
		Size: 46.8 MB (46840961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2880df797d0653bf59426d2fef27e7c6fdb9bb8b8aa0c402b64feac76a60c9a0`  
		Last Modified: Tue, 07 Jun 2022 00:22:57 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfe78a9f6b3a86975d0e84bb3161732e5ba01285bb1a6ae73bb954bd7265674`  
		Last Modified: Tue, 07 Jun 2022 05:36:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58004d6f9a4171ea223dc2112ecba8a0f76ac3f1cbc06be1a14d1ead6ee5f867`  
		Last Modified: Tue, 07 Jun 2022 05:36:21 GMT  
		Size: 3.7 MB (3660191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2024ed319db54955606f82a59f3fa9bc2ecc33041e08ce892b7f570543b95dd6`  
		Last Modified: Tue, 07 Jun 2022 05:36:20 GMT  
		Size: 62.9 KB (62886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267e75816020eb40ff1b95d79eb8668420d23365e2c734b529532af7edfdcecd`  
		Last Modified: Tue, 07 Jun 2022 05:59:25 GMT  
		Size: 65.6 MB (65607730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomee:9-microprofile` - linux; arm64 variant v8

```console
$ docker pull tomee@sha256:789a19ec2ff2137dbb7746f4a37ee3d84fa28f97ff38c8dcf5bbfda1ef13bb64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.0 MB (163010209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aff8ff8102a5e5984a8172e3a0e5a0defaad3f4fac4fa564f7eaee206d03921`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:28:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:30:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:30:47 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Fri, 29 Apr 2022 23:31:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 29 Apr 2022 23:31:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Apr 2022 23:31:30 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 24 May 2022 17:44:13 GMT
ENV PATH=/usr/local/tomee/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 May 2022 17:44:13 GMT
RUN mkdir -p /usr/local/tomee
# Tue, 24 May 2022 17:44:14 GMT
WORKDIR /usr/local/tomee
# Tue, 24 May 2022 17:44:24 GMT
RUN apt-get update   && apt-get install -y  gpg   && rm -rf /var/lib/apt/lists/*
# Tue, 24 May 2022 17:44:33 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   B83D15E72253ED1104EB4FBBDAB472F0E5B8A431   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Tue, 24 May 2022 17:53:22 GMT
ENV TOMEE_VER=9.0.0-M7
# Tue, 24 May 2022 17:53:59 GMT
ENV TOMEE_BUILD=microprofile
# Tue, 24 May 2022 17:54:06 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Tue, 24 May 2022 17:54:07 GMT
EXPOSE 8080
# Tue, 24 May 2022 17:54:07 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b467f4b58f0fff42ab91803fe1a7c56675eed1a58f67991e9e7b0e445b91c1`  
		Last Modified: Fri, 29 Apr 2022 23:35:19 GMT  
		Size: 20.5 MB (20499354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec67f097ff34e42214a096abc801c87c94bf54ec712dd7c8c7cfa9c4cce2294`  
		Last Modified: Fri, 29 Apr 2022 23:36:00 GMT  
		Size: 46.3 MB (46273208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bba9689c028433e009befa69f8a6455447aa1ec9b056853669def5568774a96`  
		Last Modified: Fri, 29 Apr 2022 23:35:53 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5089e7636b98220b68493ef86febec29cb097b8d7d63fcae6f890a8c352c3cee`  
		Last Modified: Tue, 24 May 2022 18:36:08 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcd11222335f999e94ec474644939e6cdb0c36e64f0ee46cc2d1f44fc9a5c34`  
		Last Modified: Tue, 24 May 2022 18:36:09 GMT  
		Size: 3.4 MB (3397649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c860bf52d044cbcecddd05b568b319f9d07329e5e44c5fb1653c1e9d4a100`  
		Last Modified: Tue, 24 May 2022 18:36:08 GMT  
		Size: 62.9 KB (62866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3a9e7fa1f25a13e4df37fce13f2f815ccbde39cc3365aa2f1c132fd741bac0`  
		Last Modified: Tue, 24 May 2022 19:02:45 GMT  
		Size: 65.6 MB (65607478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
