## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:9fcc2a11d8d74b0f2ba626a7ef6fed1c5c754282c41f0a2f3fad34872ab3893d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:d63c821c2971ded29ad0185d23637a706bdac4a50b2867fa38ea5cb9ff8ffcb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1928375857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8047e98f297852604ef2f8268858f0075d3769ed50df4172152065bbfa78cdd`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:43:58 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Tue, 25 Oct 2022 17:43:58 GMT
ENV TERM=xterm
# Tue, 25 Oct 2022 17:50:41 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Tue, 25 Oct 2022 17:50:52 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Tue, 25 Oct 2022 17:50:59 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Tue, 25 Oct 2022 17:50:59 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Tue, 25 Oct 2022 17:51:40 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Tue, 25 Oct 2022 17:51:40 GMT
ENV LANG=en_US.UTF-8
# Tue, 25 Oct 2022 17:51:40 GMT
ENV LANGUAGE=en_US.UTF-8
# Tue, 25 Oct 2022 17:51:41 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 17:51:41 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 25 Oct 2022 17:51:42 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 25 Oct 2022 17:51:42 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 25 Oct 2022 17:51:42 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Tue, 25 Oct 2022 17:51:42 GMT
ENV JBOSS_HOME=/opt/wildfly
# Tue, 25 Oct 2022 17:51:42 GMT
ENV SILVERPEAS_VERSION=6.3
# Tue, 25 Oct 2022 17:51:42 GMT
ENV WILDFLY_VERSION=26.1.1
# Tue, 25 Oct 2022 17:51:42 GMT
LABEL name=Silverpeas 6.3 description=Image to install and to run Silverpeas 6.3 vendor=Silverpeas version=6.3 build=1
# Tue, 25 Oct 2022 18:04:17 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver keys.openpgp.org --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Tue, 25 Oct 2022 18:04:18 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Tue, 25 Oct 2022 18:04:18 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Tue, 25 Oct 2022 18:04:18 GMT
WORKDIR /opt/silverpeas/bin
# Tue, 25 Oct 2022 18:04:18 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Tue, 25 Oct 2022 18:04:19 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Tue, 25 Oct 2022 18:09:14 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Tue, 25 Oct 2022 18:09:17 GMT
EXPOSE 8000 9990
# Tue, 25 Oct 2022 18:09:18 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Tue, 25 Oct 2022 18:09:18 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0571772de86ccccc2a3900d857b2b7dddfdbdd05e63f8f15480f86046c91079`  
		Last Modified: Tue, 25 Oct 2022 18:27:34 GMT  
		Size: 911.1 MB (911064637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60227ce57d3303a4189eacc0efc8261cf50d1534a7b7f3248c27fecf0a9a724d`  
		Last Modified: Tue, 25 Oct 2022 18:23:57 GMT  
		Size: 4.0 MB (3994069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e5985d602c308be9e930825b2cd8c0fa0f1af2c8f2799c74df9855445330b2`  
		Last Modified: Tue, 25 Oct 2022 18:23:58 GMT  
		Size: 7.1 MB (7146638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d05d0865aa62b6e52910a9d1a1f73401a651a0141c0bf746b9163e2cef8d545`  
		Last Modified: Tue, 25 Oct 2022 18:23:55 GMT  
		Size: 2.5 MB (2534354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5c768a438b82df35db7008514d9564551c686fc61296d42ab0781cfd307792`  
		Last Modified: Tue, 25 Oct 2022 18:23:54 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcba6622f5215f590677b23d20c1a8c9823a90fe9729f34b180b8a27ff7c0ce`  
		Last Modified: Tue, 25 Oct 2022 18:23:55 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8a13875f4df0720eaaf5f1e67f9c98d665ab2673e4a8a644e752a2c6edd9c7`  
		Last Modified: Tue, 25 Oct 2022 18:24:07 GMT  
		Size: 217.8 MB (217842829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9449910b28cfd7d8ac860459de891013d4042abc76bacb69f127ba5ec3cafae9`  
		Last Modified: Tue, 25 Oct 2022 18:23:53 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99557035a1904ce84c51391e22e77bf4f622e6e8fbd1b1e1520ff397aa44c9d`  
		Last Modified: Tue, 25 Oct 2022 18:23:52 GMT  
		Size: 664.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97befa548964c0c5a9395289415f97339446d23a9304ab60b8b19218bac240d`  
		Last Modified: Tue, 25 Oct 2022 18:23:52 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93d542de0fde9854d0f429e327d4da75a66a78e3aba65bfb255928bef2e0e7b`  
		Last Modified: Tue, 25 Oct 2022 18:23:52 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeff16ecc9fca187fd869636cdf64bc67da75fb3de5ad5de6ccc72287c1cb4f`  
		Last Modified: Tue, 25 Oct 2022 18:24:42 GMT  
		Size: 757.2 MB (757212789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
