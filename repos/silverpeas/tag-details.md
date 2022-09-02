<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `silverpeas`

-	[`silverpeas:6.2.3`](#silverpeas623)
-	[`silverpeas:latest`](#silverpeaslatest)

## `silverpeas:6.2.3`

```console
$ docker pull silverpeas@sha256:971c1a5a80c46b3c1ccf762f665841505df52488782bbcd999cd79587d85ba8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:6.2.3` - linux; amd64

```console
$ docker pull silverpeas@sha256:96246abd5c3236fd7f4e94650298109f61944ab8d68bfb3efb4d95bd7566b491
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1898143188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f49dfb905a1564c8f23d8f911f989612b803696b1e6140339199dc3ee0ae33be`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:34:27 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Fri, 02 Sep 2022 05:34:27 GMT
ENV TERM=xterm
# Fri, 02 Sep 2022 05:42:09 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Fri, 02 Sep 2022 05:42:24 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Fri, 02 Sep 2022 05:42:30 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Fri, 02 Sep 2022 05:42:30 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Fri, 02 Sep 2022 05:43:10 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Fri, 02 Sep 2022 05:43:10 GMT
ENV LANG=en_US.UTF-8
# Fri, 02 Sep 2022 05:43:10 GMT
ENV LANGUAGE=en_US.UTF-8
# Fri, 02 Sep 2022 05:43:10 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 02 Sep 2022 05:43:10 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 02 Sep 2022 05:43:11 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 02 Sep 2022 05:43:11 GMT
ENV JAVA_HOME=/docker-java-home
# Fri, 02 Sep 2022 05:43:11 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Fri, 02 Sep 2022 05:43:11 GMT
ENV JBOSS_HOME=/opt/wildfly
# Fri, 02 Sep 2022 05:43:11 GMT
ENV SILVERPEAS_VERSION=6.2.3
# Fri, 02 Sep 2022 05:43:11 GMT
ENV WILDFLY_VERSION=20.0.1
# Fri, 02 Sep 2022 05:43:12 GMT
LABEL name=Silverpeas 6.2.3 description=Image to install and to run Silverpeas 6.2.3 vendor=Silverpeas version=6.2.3 build=1
# Fri, 02 Sep 2022 05:43:56 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver keys.openpgp.org --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Fri, 02 Sep 2022 05:43:57 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Fri, 02 Sep 2022 05:43:57 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Fri, 02 Sep 2022 05:43:57 GMT
WORKDIR /opt/silverpeas/bin
# Fri, 02 Sep 2022 05:43:57 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Fri, 02 Sep 2022 05:43:57 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Fri, 02 Sep 2022 05:45:58 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Fri, 02 Sep 2022 05:46:01 GMT
EXPOSE 8000 9990
# Fri, 02 Sep 2022 05:46:01 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Fri, 02 Sep 2022 05:46:02 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245516d9e0ba23ce361cb2270092774c8b2d75a061fdd5c31f9013a67db4d1d8`  
		Last Modified: Fri, 02 Sep 2022 05:47:50 GMT  
		Size: 911.0 MB (911044934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92b35ccaee67b25b31ab680c6ea0026f206fa4875cac955138c1ffc64abc1d9`  
		Last Modified: Fri, 02 Sep 2022 05:46:17 GMT  
		Size: 4.0 MB (3994067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827e4164bbdd689ee13f074e903488f4ba28416b47a0bfa17ef3f107f72d6acb`  
		Last Modified: Fri, 02 Sep 2022 05:46:17 GMT  
		Size: 7.1 MB (7146633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f71faa73bc2cf7d4eeef2afcf2bf92ab49646c1a4a49d5e722b431fe9f6dc1`  
		Last Modified: Fri, 02 Sep 2022 05:46:14 GMT  
		Size: 2.5 MB (2534367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5886cd1bb0d58a7769a964f1e95325ad150042e36ae881d91c7769db26126e01`  
		Last Modified: Fri, 02 Sep 2022 05:46:14 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b95ae1bfd295814dfcb518ad8dd1d152d8da02b465375ce3326cb3c42211381`  
		Last Modified: Fri, 02 Sep 2022 05:46:14 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12caef4c4bebc2f94bef6abd6290d0eb6438286e0e47683c9b41cd4bee3a0ca1`  
		Last Modified: Fri, 02 Sep 2022 05:46:26 GMT  
		Size: 196.8 MB (196774082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5feef1aeaea9a38febdb144b1a262a01c454dbead40fc4379d6741d8b975a449`  
		Last Modified: Fri, 02 Sep 2022 05:46:12 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ab3ef7800af058a6b5a48f4694eb4d5a77ac32b02cc07095ac860cc0c251ce`  
		Last Modified: Fri, 02 Sep 2022 05:46:12 GMT  
		Size: 662.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3579b027eea85a7cf7526608aae4b0f14bb1aa82375dfb9e6bd9ebb84f1e9f76`  
		Last Modified: Fri, 02 Sep 2022 05:46:12 GMT  
		Size: 876.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c88b84cc41699c1a0361fd6c28a4ce79e8c6d4207923a7bfc51e3ec903724a`  
		Last Modified: Fri, 02 Sep 2022 05:46:12 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ae0eb8467775521cf4038498a54f05466d5bf5557b4aead806c8079f267984`  
		Last Modified: Fri, 02 Sep 2022 05:46:49 GMT  
		Size: 748.1 MB (748073717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:971c1a5a80c46b3c1ccf762f665841505df52488782bbcd999cd79587d85ba8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:96246abd5c3236fd7f4e94650298109f61944ab8d68bfb3efb4d95bd7566b491
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1898143188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f49dfb905a1564c8f23d8f911f989612b803696b1e6140339199dc3ee0ae33be`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:34:27 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Fri, 02 Sep 2022 05:34:27 GMT
ENV TERM=xterm
# Fri, 02 Sep 2022 05:42:09 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Fri, 02 Sep 2022 05:42:24 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Fri, 02 Sep 2022 05:42:30 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Fri, 02 Sep 2022 05:42:30 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Fri, 02 Sep 2022 05:43:10 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Fri, 02 Sep 2022 05:43:10 GMT
ENV LANG=en_US.UTF-8
# Fri, 02 Sep 2022 05:43:10 GMT
ENV LANGUAGE=en_US.UTF-8
# Fri, 02 Sep 2022 05:43:10 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 02 Sep 2022 05:43:10 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 02 Sep 2022 05:43:11 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 02 Sep 2022 05:43:11 GMT
ENV JAVA_HOME=/docker-java-home
# Fri, 02 Sep 2022 05:43:11 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Fri, 02 Sep 2022 05:43:11 GMT
ENV JBOSS_HOME=/opt/wildfly
# Fri, 02 Sep 2022 05:43:11 GMT
ENV SILVERPEAS_VERSION=6.2.3
# Fri, 02 Sep 2022 05:43:11 GMT
ENV WILDFLY_VERSION=20.0.1
# Fri, 02 Sep 2022 05:43:12 GMT
LABEL name=Silverpeas 6.2.3 description=Image to install and to run Silverpeas 6.2.3 vendor=Silverpeas version=6.2.3 build=1
# Fri, 02 Sep 2022 05:43:56 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver keys.openpgp.org --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Fri, 02 Sep 2022 05:43:57 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Fri, 02 Sep 2022 05:43:57 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Fri, 02 Sep 2022 05:43:57 GMT
WORKDIR /opt/silverpeas/bin
# Fri, 02 Sep 2022 05:43:57 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Fri, 02 Sep 2022 05:43:57 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Fri, 02 Sep 2022 05:45:58 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Fri, 02 Sep 2022 05:46:01 GMT
EXPOSE 8000 9990
# Fri, 02 Sep 2022 05:46:01 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Fri, 02 Sep 2022 05:46:02 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245516d9e0ba23ce361cb2270092774c8b2d75a061fdd5c31f9013a67db4d1d8`  
		Last Modified: Fri, 02 Sep 2022 05:47:50 GMT  
		Size: 911.0 MB (911044934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92b35ccaee67b25b31ab680c6ea0026f206fa4875cac955138c1ffc64abc1d9`  
		Last Modified: Fri, 02 Sep 2022 05:46:17 GMT  
		Size: 4.0 MB (3994067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827e4164bbdd689ee13f074e903488f4ba28416b47a0bfa17ef3f107f72d6acb`  
		Last Modified: Fri, 02 Sep 2022 05:46:17 GMT  
		Size: 7.1 MB (7146633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f71faa73bc2cf7d4eeef2afcf2bf92ab49646c1a4a49d5e722b431fe9f6dc1`  
		Last Modified: Fri, 02 Sep 2022 05:46:14 GMT  
		Size: 2.5 MB (2534367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5886cd1bb0d58a7769a964f1e95325ad150042e36ae881d91c7769db26126e01`  
		Last Modified: Fri, 02 Sep 2022 05:46:14 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b95ae1bfd295814dfcb518ad8dd1d152d8da02b465375ce3326cb3c42211381`  
		Last Modified: Fri, 02 Sep 2022 05:46:14 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12caef4c4bebc2f94bef6abd6290d0eb6438286e0e47683c9b41cd4bee3a0ca1`  
		Last Modified: Fri, 02 Sep 2022 05:46:26 GMT  
		Size: 196.8 MB (196774082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5feef1aeaea9a38febdb144b1a262a01c454dbead40fc4379d6741d8b975a449`  
		Last Modified: Fri, 02 Sep 2022 05:46:12 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ab3ef7800af058a6b5a48f4694eb4d5a77ac32b02cc07095ac860cc0c251ce`  
		Last Modified: Fri, 02 Sep 2022 05:46:12 GMT  
		Size: 662.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3579b027eea85a7cf7526608aae4b0f14bb1aa82375dfb9e6bd9ebb84f1e9f76`  
		Last Modified: Fri, 02 Sep 2022 05:46:12 GMT  
		Size: 876.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c88b84cc41699c1a0361fd6c28a4ce79e8c6d4207923a7bfc51e3ec903724a`  
		Last Modified: Fri, 02 Sep 2022 05:46:12 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ae0eb8467775521cf4038498a54f05466d5bf5557b4aead806c8079f267984`  
		Last Modified: Fri, 02 Sep 2022 05:46:49 GMT  
		Size: 748.1 MB (748073717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
