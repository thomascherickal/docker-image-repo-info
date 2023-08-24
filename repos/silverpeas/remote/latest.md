## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:18f412a433db363cc10f2fe2eca07d1955c486c9288e6d6f576961ed57362e11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:ca9b3a9ceb1630a98ee61601654d73bd4af3a046223e56a4cee8be2e1585bd24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1780746784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0df5dcfb2a6cf94274f1407d52d63df6708932e604320f2a0e3ed3cb5708da3`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 17 Aug 2023 07:05:27 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Thu, 17 Aug 2023 07:05:27 GMT
ENV TERM=xterm
# Thu, 17 Aug 2023 07:13:17 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Thu, 17 Aug 2023 07:13:24 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Thu, 17 Aug 2023 07:13:27 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Thu, 17 Aug 2023 07:13:27 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Thu, 17 Aug 2023 07:14:05 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Thu, 17 Aug 2023 07:14:05 GMT
ENV LANG=en_US.UTF-8
# Thu, 17 Aug 2023 07:14:05 GMT
ENV LANGUAGE=en_US.UTF-8
# Thu, 17 Aug 2023 07:14:05 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 17 Aug 2023 07:14:06 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 17 Aug 2023 07:14:06 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 17 Aug 2023 07:14:06 GMT
ENV JAVA_HOME=/docker-java-home
# Thu, 17 Aug 2023 07:14:06 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Thu, 17 Aug 2023 07:14:06 GMT
ENV JBOSS_HOME=/opt/wildfly
# Thu, 24 Aug 2023 19:20:18 GMT
ENV SILVERPEAS_VERSION=6.3.1
# Thu, 24 Aug 2023 19:20:18 GMT
ENV WILDFLY_VERSION=26.1.1
# Thu, 24 Aug 2023 19:20:18 GMT
LABEL name=Silverpeas 6.3.1 description=Image to install and to run Silverpeas 6.3.1 vendor=Silverpeas version=6.3.1 build=1
# Thu, 24 Aug 2023 19:20:55 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver keys.openpgp.org --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Thu, 24 Aug 2023 19:20:55 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Thu, 24 Aug 2023 19:20:55 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Thu, 24 Aug 2023 19:20:55 GMT
WORKDIR /opt/silverpeas/bin
# Thu, 24 Aug 2023 19:20:56 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Thu, 24 Aug 2023 19:20:56 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Thu, 24 Aug 2023 19:23:37 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Thu, 24 Aug 2023 19:23:40 GMT
EXPOSE 8000 9990
# Thu, 24 Aug 2023 19:23:40 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Thu, 24 Aug 2023 19:23:40 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464a79e0944ca89e87d9ba42f2eb625d6e9213eb3150c86cbff33ee3cba42f4f`  
		Last Modified: Thu, 17 Aug 2023 07:20:31 GMT  
		Size: 762.3 MB (762278845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e0a7905a224a8523ddcc11f1cad48de7cd5eeddd1289e5ea553268aa56b953`  
		Last Modified: Thu, 17 Aug 2023 07:19:12 GMT  
		Size: 4.0 MB (3994089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31f9118ab954f9221b04b9a5176bf9ed1fb19837635bbd83fc514aa28d33bab`  
		Last Modified: Thu, 17 Aug 2023 07:19:13 GMT  
		Size: 7.1 MB (7146666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ebc7fc6cfa041874d5e8f31cc112e5a2eb2440c4b4a990253da2af1af8a4c5`  
		Last Modified: Thu, 17 Aug 2023 07:19:10 GMT  
		Size: 2.5 MB (2534358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8d31dfd233901e80804159ee34237b080f20dce537d0d58b23def3f724652`  
		Last Modified: Thu, 17 Aug 2023 07:19:09 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56f3732208ac9e291674aab83df5f56690d580ad305f11ed140bba761a9a72d`  
		Last Modified: Thu, 17 Aug 2023 07:19:09 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a26886b732e16d0952cf5830d3d5beea34b48c1177871efdcfc6d6f6e6bfa6`  
		Last Modified: Thu, 24 Aug 2023 19:24:21 GMT  
		Size: 217.8 MB (217842732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd71b3d3d9db5209ae5d45f640cafdbddd14894df373a4e21a290d901b931e1`  
		Last Modified: Thu, 24 Aug 2023 19:24:06 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e349db82bcf24556811a3766128b0388bf6d3f1de83d8d309ba470b1aa8f8a`  
		Last Modified: Thu, 24 Aug 2023 19:24:06 GMT  
		Size: 663.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d453606d2024b215b16e299b5757740bd426e323491bd6bf375c6e0d3360b8e2`  
		Last Modified: Thu, 24 Aug 2023 19:24:06 GMT  
		Size: 875.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d5144b357e53ba59fe1bfaef5a3771d74e804f89ac13855816dc4802498abe`  
		Last Modified: Thu, 24 Aug 2023 19:24:05 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854b79dc36109567c2dedab87b47af43d8f6f0bacba61763a62598210a75313f`  
		Last Modified: Thu, 24 Aug 2023 19:24:40 GMT  
		Size: 758.4 MB (758366722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
