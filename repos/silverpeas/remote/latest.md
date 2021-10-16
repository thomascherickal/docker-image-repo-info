## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:7d115b28c44604e9b8e23e3142e149312202e7ee2da440d92feca26c9ef7357d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:e61500a9b9667b97f993f5d9dc7ad94067a8200ae50cd53a040220cb0e30f46c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1889282059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92894ed5fd296d1a7e5a379a3be910f468d6bc50dc6fe5b09b1e89ee7a6a1405`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:13:25 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Sat, 16 Oct 2021 03:13:26 GMT
ENV TERM=xterm
# Sat, 16 Oct 2021 03:19:54 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Sat, 16 Oct 2021 03:20:00 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Sat, 16 Oct 2021 03:20:05 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Sat, 16 Oct 2021 03:20:05 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Sat, 16 Oct 2021 03:20:44 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Sat, 16 Oct 2021 03:20:44 GMT
ENV LANG=en_US.UTF-8
# Sat, 16 Oct 2021 03:20:44 GMT
ENV LANGUAGE=en_US.UTF-8
# Sat, 16 Oct 2021 03:20:44 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 03:20:45 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 16 Oct 2021 03:20:46 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 16 Oct 2021 03:20:46 GMT
ENV JAVA_HOME=/docker-java-home
# Sat, 16 Oct 2021 03:20:46 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Sat, 16 Oct 2021 03:20:46 GMT
ENV JBOSS_HOME=/opt/wildfly
# Sat, 16 Oct 2021 03:20:47 GMT
ENV SILVERPEAS_VERSION=6.2.1
# Sat, 16 Oct 2021 03:20:47 GMT
ENV WILDFLY_VERSION=20.0.1
# Sat, 16 Oct 2021 03:20:47 GMT
LABEL name=Silverpeas 6.2.1 description=Image to install and to run Silverpeas 6.2.1 vendor=Silverpeas version=6.2.1 build=1
# Sat, 16 Oct 2021 03:21:07 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Sat, 16 Oct 2021 03:21:08 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Sat, 16 Oct 2021 03:21:08 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Sat, 16 Oct 2021 03:21:08 GMT
WORKDIR /opt/silverpeas/bin
# Sat, 16 Oct 2021 03:21:08 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Sat, 16 Oct 2021 03:21:09 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Sat, 16 Oct 2021 03:23:26 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Sat, 16 Oct 2021 03:23:29 GMT
EXPOSE 8000 9990
# Sat, 16 Oct 2021 03:23:29 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Sat, 16 Oct 2021 03:23:30 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200d878df30075fcecb4d08f2e50d8ae1652fd84ff4d249ee0ddd4ee484d5951`  
		Last Modified: Sat, 16 Oct 2021 03:25:24 GMT  
		Size: 909.8 MB (909802898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebbf7f2028d16c581936c5f39680eb21f6aa038e9b06b4a8cdeb12e08593779`  
		Last Modified: Sat, 16 Oct 2021 03:23:51 GMT  
		Size: 4.0 MB (3994070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea30ec91ca3e147ceabea6d7511b77c16ded4c11c43899d1e4b3aa9df4f214f`  
		Last Modified: Sat, 16 Oct 2021 03:23:51 GMT  
		Size: 7.1 MB (7146660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670dfa300b7144e3bad0666e98c37f53d0826075b99ad5292a607829b6262cd7`  
		Last Modified: Sat, 16 Oct 2021 03:23:48 GMT  
		Size: 2.5 MB (2534365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744477919b53b641498abaffbe0cab93a5bd7cea050e60f57a3885c4ae620f10`  
		Last Modified: Sat, 16 Oct 2021 03:23:47 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2140c07c7f8f9cb94b1a699e73c99546797fa149b5eb0bf33b7d6e7c46e95c57`  
		Last Modified: Sat, 16 Oct 2021 03:23:47 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81235eb81b3ae9e751176d94aae14ef68496b3677ad2428b98386f832bfc795`  
		Last Modified: Sat, 16 Oct 2021 03:24:00 GMT  
		Size: 196.8 MB (196774084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7af7060ba7c73388d5b8faeb5bdcef244f834d132ef6bc89e610c8155284fce`  
		Last Modified: Sat, 16 Oct 2021 03:23:45 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9b128f2b6eb6208385ac02106958e3e3b48210485070265b51f5c351f20b96`  
		Last Modified: Sat, 16 Oct 2021 03:23:45 GMT  
		Size: 663.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f90bb32e8fd75f518e2ee7252325891bab7ea0f4c79ee784302dd7c2af3cb1`  
		Last Modified: Sat, 16 Oct 2021 03:23:45 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d41b40eb992b675c4f29a0393d4f60eef077d294af961abc1bc2fa576a224fd`  
		Last Modified: Sat, 16 Oct 2021 03:23:45 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7dc94c49bce327464b7fbb93d9141f62327cae66544154c6492d2cf766fdd5`  
		Last Modified: Sat, 16 Oct 2021 03:24:23 GMT  
		Size: 740.5 MB (740460178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
