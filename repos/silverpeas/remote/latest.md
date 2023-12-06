## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:b2dc6bd665bea5d01684531c757d9cd1aadeb544c0b576424cbc8ee3c311c18c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:48b2ff93e2f943f36ad4a40ea75a18bafc20c6bc005d5462ee533b52583035a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1780884748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7af9ff3b47c8af3fd9d9dea50619f760a34fbd9dc26b96fd7660fd11c43e2933`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:31:30 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Sat, 02 Dec 2023 06:31:30 GMT
ENV TERM=xterm
# Sat, 02 Dec 2023 06:40:33 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Sat, 02 Dec 2023 06:40:42 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Sat, 02 Dec 2023 06:40:47 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Sat, 02 Dec 2023 06:40:47 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Sat, 02 Dec 2023 06:41:25 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Sat, 02 Dec 2023 06:41:25 GMT
ENV LANG=en_US.UTF-8
# Sat, 02 Dec 2023 06:41:25 GMT
ENV LANGUAGE=en_US.UTF-8
# Sat, 02 Dec 2023 06:41:25 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:41:26 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 02 Dec 2023 06:41:26 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 02 Dec 2023 06:41:26 GMT
ENV JAVA_HOME=/docker-java-home
# Sat, 02 Dec 2023 06:41:26 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Sat, 02 Dec 2023 06:41:27 GMT
ENV JBOSS_HOME=/opt/wildfly
# Wed, 06 Dec 2023 19:24:56 GMT
ENV SILVERPEAS_VERSION=6.3.3
# Wed, 06 Dec 2023 19:24:56 GMT
ENV WILDFLY_VERSION=26.1.1
# Wed, 06 Dec 2023 19:24:56 GMT
LABEL name=Silverpeas 6.3.3 description=Image to install and to run Silverpeas 6.3.3 vendor=Silverpeas version=6.3.3 build=1
# Wed, 06 Dec 2023 19:41:02 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver keys.openpgp.org --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Wed, 06 Dec 2023 19:41:03 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Wed, 06 Dec 2023 19:41:03 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Wed, 06 Dec 2023 19:41:03 GMT
WORKDIR /opt/silverpeas/bin
# Wed, 06 Dec 2023 19:41:03 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Wed, 06 Dec 2023 19:41:03 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Wed, 06 Dec 2023 19:46:58 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Wed, 06 Dec 2023 19:47:01 GMT
EXPOSE 8000 9990
# Wed, 06 Dec 2023 19:47:01 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Wed, 06 Dec 2023 19:47:01 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df5608df20cb6a703c4c249d37ee7202a913bf956332c7e3b6fa49ac8ddbc57`  
		Last Modified: Sat, 02 Dec 2023 06:52:49 GMT  
		Size: 762.4 MB (762357323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2cc1d8ab965ebf39cd37a6290af75654fe271367532df5e5ca3d7d33bbb3cc`  
		Last Modified: Sat, 02 Dec 2023 06:51:29 GMT  
		Size: 4.0 MB (3994076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae6ed185b7f7a10fef3c653721c6270545c578b643affff73b1776c538a1839`  
		Last Modified: Sat, 02 Dec 2023 06:51:29 GMT  
		Size: 7.1 MB (7146661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d04e77484d5dc6e0cf6a722e2b32b1c88c573ec9517e8375ba5144dab5b2d7`  
		Last Modified: Sat, 02 Dec 2023 06:51:27 GMT  
		Size: 2.5 MB (2534355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911599266d2a70fdd860cdea1db05ba2b1de3420824bcc4ede99ace6d090ae2e`  
		Last Modified: Sat, 02 Dec 2023 06:51:26 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e689f539cf2cfd5c3216446f9b13acad7e32785f8cd653492cd72b51ba5134`  
		Last Modified: Sat, 02 Dec 2023 06:51:26 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fffdbb5a383d5493c068886b152bbf74ba35c40da1b93df18d78e199bddeeb`  
		Last Modified: Wed, 06 Dec 2023 19:47:29 GMT  
		Size: 217.8 MB (217842746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe1c3924f0cdc05080e6e6caf339b781a6af8545b19c7417c03429ce5681f14`  
		Last Modified: Wed, 06 Dec 2023 19:47:13 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aafc59573d2603fc92e28bb357a7dfe0e3776adcefb2ae8f55a8538198bddcb`  
		Last Modified: Wed, 06 Dec 2023 19:47:14 GMT  
		Size: 663.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79c3f16f796f758b5f62c2d739f170d75da450a1dba51e009654aaca7eb58ef`  
		Last Modified: Wed, 06 Dec 2023 19:47:14 GMT  
		Size: 876.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2795c57ab3abc4709b11dfeb276fa1c114a760e653843345e8c4ccd14d9b18`  
		Last Modified: Wed, 06 Dec 2023 19:47:13 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2c9fefbc1a908431ff07c95f68364439f408df746588301e04b87f4ba81226`  
		Last Modified: Wed, 06 Dec 2023 19:47:47 GMT  
		Size: 758.4 MB (758422851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
