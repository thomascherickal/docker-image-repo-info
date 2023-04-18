<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `silverpeas`

-	[`silverpeas:6.2.3-b1`](#silverpeas623-b1)
-	[`silverpeas:6.3`](#silverpeas63)
-	[`silverpeas:latest`](#silverpeaslatest)

## `silverpeas:6.2.3-b1`

```console
$ docker pull silverpeas@sha256:ade48bb2e1cbc0b6265537515e6fcd8d1317a269a36ef6978aba28adaf5fee84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:6.2.3-b1` - linux; amd64

```console
$ docker pull silverpeas@sha256:58a85306c54bff1160927c4e302e270330388ec29200d879177d4b3aa9feca63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1898398313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c946efb1c9ae0ad8a3b82ca8a7b5923458f6fc6c46c17643fd8028a12e87692d`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:03:53 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Thu, 16 Mar 2023 05:03:53 GMT
ENV TERM=xterm
# Thu, 16 Mar 2023 05:11:38 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Thu, 16 Mar 2023 05:11:43 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Thu, 16 Mar 2023 05:11:47 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Thu, 16 Mar 2023 05:11:47 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Thu, 16 Mar 2023 05:12:27 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Thu, 16 Mar 2023 05:12:27 GMT
ENV LANG=en_US.UTF-8
# Thu, 16 Mar 2023 05:12:27 GMT
ENV LANGUAGE=en_US.UTF-8
# Thu, 16 Mar 2023 05:12:27 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 05:12:28 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 16 Mar 2023 05:12:28 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 16 Mar 2023 05:12:28 GMT
ENV JAVA_HOME=/docker-java-home
# Thu, 16 Mar 2023 05:12:28 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Thu, 16 Mar 2023 05:12:29 GMT
ENV JBOSS_HOME=/opt/wildfly
# Thu, 16 Mar 2023 05:15:47 GMT
ENV SILVERPEAS_VERSION=6.2.3
# Thu, 16 Mar 2023 05:15:48 GMT
ENV WILDFLY_VERSION=20.0.1
# Thu, 16 Mar 2023 05:15:48 GMT
LABEL name=Silverpeas 6.2.3 description=Image to install and to run Silverpeas 6.2.3 vendor=Silverpeas version=6.2.3 build=2
# Thu, 16 Mar 2023 05:16:31 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver keys.openpgp.org --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://silverpeas.org/files/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Thu, 16 Mar 2023 05:16:31 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Thu, 16 Mar 2023 05:16:31 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Thu, 16 Mar 2023 05:16:32 GMT
WORKDIR /opt/silverpeas/bin
# Thu, 16 Mar 2023 05:16:32 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Thu, 16 Mar 2023 05:16:32 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Thu, 16 Mar 2023 05:18:14 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Thu, 16 Mar 2023 05:18:17 GMT
EXPOSE 8000 9990
# Thu, 16 Mar 2023 05:18:17 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Thu, 16 Mar 2023 05:18:17 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c885a708406aa378c5f79799ec1f8903a7ed1d86f5e9d4cf8e60502c17f858`  
		Last Modified: Thu, 16 Mar 2023 05:20:04 GMT  
		Size: 911.3 MB (911294931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5255a1fd2d32df994cafba9a64b818c786c0a604afb1d1e29255a1d6813e48`  
		Last Modified: Thu, 16 Mar 2023 05:18:36 GMT  
		Size: 4.0 MB (3994069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86be06c1337bf564070e4d861c22c213104e4adc63b26d4baa3deb5ff499fc32`  
		Last Modified: Thu, 16 Mar 2023 05:18:37 GMT  
		Size: 7.1 MB (7146637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98f67ac5b10aeddb812a368e777e01b164e428e13baee512f0ac7008ab65a4d`  
		Last Modified: Thu, 16 Mar 2023 05:18:34 GMT  
		Size: 2.5 MB (2534360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592a0230c0856f215d02f7c9bbe6f04d854248f50818b0c88d8f896164fcbe23`  
		Last Modified: Thu, 16 Mar 2023 05:18:33 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f92a8a55ec1d2f27442125a2719d6ea6fc09aec7c980b7852924604943e670`  
		Last Modified: Thu, 16 Mar 2023 05:18:33 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966dfdf4a73b508945c639a80a2528524539fcae06ca81a9df5428a72f2474b1`  
		Last Modified: Thu, 16 Mar 2023 05:20:26 GMT  
		Size: 196.8 MB (196774113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cf8c96e8cd952bde30e1191d67449eeef704e0f77c2c976c4e6019f1b7b6fc`  
		Last Modified: Thu, 16 Mar 2023 05:20:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d238f143d42bad2f239a01df496b7bce5bf86138e6cc024cb98e1180d4dc07`  
		Last Modified: Thu, 16 Mar 2023 05:20:14 GMT  
		Size: 661.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa1163c2999dac96500fa472282b2632538daffa41aae3a6d4f46186ba3f1a4`  
		Last Modified: Thu, 16 Mar 2023 05:20:14 GMT  
		Size: 875.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c54f788b4ff423b3ad7cd4343553df430ab7ef1d512f6ebe15bf18fe9942723`  
		Last Modified: Thu, 16 Mar 2023 05:20:14 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcf87932f62ec5804023e9d767bb21e94ac3304f412ab0e681c7d3303e9b301`  
		Last Modified: Thu, 16 Mar 2023 05:20:46 GMT  
		Size: 748.1 MB (748073437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:6.3`

```console
$ docker pull silverpeas@sha256:662522ee79834aa2623117872e35416e422c56cd5c1b09d7af993a5dbd433243
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:6.3` - linux; amd64

```console
$ docker pull silverpeas@sha256:cc705b566e404cc20968f6b4981e7dd3f0b893f6df2e79e2f6cd1d6f5607fa98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1928674079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7402d5c4bc253b5ee02698c8d37c6af11e7a3d5f8bc2efb4dae8c63c5fc48c9d`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:47:35 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Tue, 18 Apr 2023 02:47:36 GMT
ENV TERM=xterm
# Tue, 18 Apr 2023 02:53:50 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Tue, 18 Apr 2023 02:54:22 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Tue, 18 Apr 2023 02:55:35 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Tue, 18 Apr 2023 02:55:35 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Tue, 18 Apr 2023 02:56:14 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Tue, 18 Apr 2023 02:56:14 GMT
ENV LANG=en_US.UTF-8
# Tue, 18 Apr 2023 02:56:15 GMT
ENV LANGUAGE=en_US.UTF-8
# Tue, 18 Apr 2023 02:56:15 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 02:56:15 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Apr 2023 02:56:16 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 18 Apr 2023 02:56:16 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 18 Apr 2023 02:56:16 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Tue, 18 Apr 2023 02:56:16 GMT
ENV JBOSS_HOME=/opt/wildfly
# Tue, 18 Apr 2023 02:56:16 GMT
ENV SILVERPEAS_VERSION=6.3
# Tue, 18 Apr 2023 02:56:16 GMT
ENV WILDFLY_VERSION=26.1.1
# Tue, 18 Apr 2023 02:56:16 GMT
LABEL name=Silverpeas 6.3 description=Image to install and to run Silverpeas 6.3 vendor=Silverpeas version=6.3 build=1
# Tue, 18 Apr 2023 03:34:13 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver keys.openpgp.org --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Tue, 18 Apr 2023 03:34:13 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Tue, 18 Apr 2023 03:34:14 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Tue, 18 Apr 2023 03:34:14 GMT
WORKDIR /opt/silverpeas/bin
# Tue, 18 Apr 2023 03:34:14 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Tue, 18 Apr 2023 03:34:14 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Tue, 18 Apr 2023 03:45:56 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Tue, 18 Apr 2023 03:45:59 GMT
EXPOSE 8000 9990
# Tue, 18 Apr 2023 03:45:59 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Tue, 18 Apr 2023 03:46:00 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade0d157f41e60b68d1a3a7b53f0ec41adad700a93015d716986e52925c25797`  
		Last Modified: Tue, 18 Apr 2023 04:50:15 GMT  
		Size: 911.4 MB (911357548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a053921dd64df31e078a8b4e794faf8f1d45280d5f8b2c406ce7f221e96e0e7`  
		Last Modified: Tue, 18 Apr 2023 04:48:49 GMT  
		Size: 4.0 MB (3994060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ea62b5e949db7db274deff6396e54b6da2be140fc5b5c12a058c54e9b1b38`  
		Last Modified: Tue, 18 Apr 2023 04:48:49 GMT  
		Size: 7.1 MB (7146639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c651e73a706a3e733e45c866697649f01f07f2b70e5f52c52a594c862ddc5f`  
		Last Modified: Tue, 18 Apr 2023 04:48:47 GMT  
		Size: 2.5 MB (2534366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61938a154e2a62cc891b77daa5c3a66a148cf7d09ce2a00ec66867cd012694df`  
		Last Modified: Tue, 18 Apr 2023 04:48:46 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb393101497fc7a58e6bebac7ac3526c1bc58a087f13b7f9e18309942d16a31`  
		Last Modified: Tue, 18 Apr 2023 04:48:46 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223d672c4b54d441cd38479c762039f2356a9b6f094034d604f686c2e4963fb9`  
		Last Modified: Tue, 18 Apr 2023 04:48:58 GMT  
		Size: 217.8 MB (217842804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128920b59aa622f754670668b188af68d3f109dd020945cfce48722b35e570c9`  
		Last Modified: Tue, 18 Apr 2023 04:48:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7c01741d80de9111ccf47708f5b96fe649713ea2adca4424f32c7e7c75c059`  
		Last Modified: Tue, 18 Apr 2023 04:48:44 GMT  
		Size: 664.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bebbdc2e415306aa55010fb30f50a251125c8f9b44e4adbd36ce711c89836ae`  
		Last Modified: Tue, 18 Apr 2023 04:48:44 GMT  
		Size: 878.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed99e84e9691c8a6d532b6ef54c1f657bc2ecba14808afcc71f7f4ed896ed44`  
		Last Modified: Tue, 18 Apr 2023 04:48:44 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fabc805858e20995b7addcbafde0edc62cdd960053e399fdbac6acc639937bd`  
		Last Modified: Tue, 18 Apr 2023 04:49:19 GMT  
		Size: 757.2 MB (757217393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:662522ee79834aa2623117872e35416e422c56cd5c1b09d7af993a5dbd433243
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:cc705b566e404cc20968f6b4981e7dd3f0b893f6df2e79e2f6cd1d6f5607fa98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1928674079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7402d5c4bc253b5ee02698c8d37c6af11e7a3d5f8bc2efb4dae8c63c5fc48c9d`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:47:35 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Tue, 18 Apr 2023 02:47:36 GMT
ENV TERM=xterm
# Tue, 18 Apr 2023 02:53:50 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Tue, 18 Apr 2023 02:54:22 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Tue, 18 Apr 2023 02:55:35 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Tue, 18 Apr 2023 02:55:35 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Tue, 18 Apr 2023 02:56:14 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Tue, 18 Apr 2023 02:56:14 GMT
ENV LANG=en_US.UTF-8
# Tue, 18 Apr 2023 02:56:15 GMT
ENV LANGUAGE=en_US.UTF-8
# Tue, 18 Apr 2023 02:56:15 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 02:56:15 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 18 Apr 2023 02:56:16 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 18 Apr 2023 02:56:16 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 18 Apr 2023 02:56:16 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Tue, 18 Apr 2023 02:56:16 GMT
ENV JBOSS_HOME=/opt/wildfly
# Tue, 18 Apr 2023 02:56:16 GMT
ENV SILVERPEAS_VERSION=6.3
# Tue, 18 Apr 2023 02:56:16 GMT
ENV WILDFLY_VERSION=26.1.1
# Tue, 18 Apr 2023 02:56:16 GMT
LABEL name=Silverpeas 6.3 description=Image to install and to run Silverpeas 6.3 vendor=Silverpeas version=6.3 build=1
# Tue, 18 Apr 2023 03:34:13 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver keys.openpgp.org --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Tue, 18 Apr 2023 03:34:13 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Tue, 18 Apr 2023 03:34:14 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Tue, 18 Apr 2023 03:34:14 GMT
WORKDIR /opt/silverpeas/bin
# Tue, 18 Apr 2023 03:34:14 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Tue, 18 Apr 2023 03:34:14 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Tue, 18 Apr 2023 03:45:56 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Tue, 18 Apr 2023 03:45:59 GMT
EXPOSE 8000 9990
# Tue, 18 Apr 2023 03:45:59 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Tue, 18 Apr 2023 03:46:00 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade0d157f41e60b68d1a3a7b53f0ec41adad700a93015d716986e52925c25797`  
		Last Modified: Tue, 18 Apr 2023 04:50:15 GMT  
		Size: 911.4 MB (911357548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a053921dd64df31e078a8b4e794faf8f1d45280d5f8b2c406ce7f221e96e0e7`  
		Last Modified: Tue, 18 Apr 2023 04:48:49 GMT  
		Size: 4.0 MB (3994060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ea62b5e949db7db274deff6396e54b6da2be140fc5b5c12a058c54e9b1b38`  
		Last Modified: Tue, 18 Apr 2023 04:48:49 GMT  
		Size: 7.1 MB (7146639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c651e73a706a3e733e45c866697649f01f07f2b70e5f52c52a594c862ddc5f`  
		Last Modified: Tue, 18 Apr 2023 04:48:47 GMT  
		Size: 2.5 MB (2534366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61938a154e2a62cc891b77daa5c3a66a148cf7d09ce2a00ec66867cd012694df`  
		Last Modified: Tue, 18 Apr 2023 04:48:46 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb393101497fc7a58e6bebac7ac3526c1bc58a087f13b7f9e18309942d16a31`  
		Last Modified: Tue, 18 Apr 2023 04:48:46 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223d672c4b54d441cd38479c762039f2356a9b6f094034d604f686c2e4963fb9`  
		Last Modified: Tue, 18 Apr 2023 04:48:58 GMT  
		Size: 217.8 MB (217842804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128920b59aa622f754670668b188af68d3f109dd020945cfce48722b35e570c9`  
		Last Modified: Tue, 18 Apr 2023 04:48:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7c01741d80de9111ccf47708f5b96fe649713ea2adca4424f32c7e7c75c059`  
		Last Modified: Tue, 18 Apr 2023 04:48:44 GMT  
		Size: 664.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bebbdc2e415306aa55010fb30f50a251125c8f9b44e4adbd36ce711c89836ae`  
		Last Modified: Tue, 18 Apr 2023 04:48:44 GMT  
		Size: 878.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed99e84e9691c8a6d532b6ef54c1f657bc2ecba14808afcc71f7f4ed896ed44`  
		Last Modified: Tue, 18 Apr 2023 04:48:44 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fabc805858e20995b7addcbafde0edc62cdd960053e399fdbac6acc639937bd`  
		Last Modified: Tue, 18 Apr 2023 04:49:19 GMT  
		Size: 757.2 MB (757217393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
