## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:7dbe407284e386f0b197001b22382253f10c6ca85711582d4ac941032a9b4bfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:14e166f4ed483178cb38adee5f6e004d72273ea0255029f0189ec4bf880b1819
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1899530255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe797bd436e0d3c77c4713181c709abf754ddec1a8fa06a74453498b37580c98`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:33 GMT
ADD file:8a50ad78a668527e974b05a3dfbfd64760de3cb643ceb8a8805d21f6ceab3389 in / 
# Thu, 03 Mar 2022 20:19:33 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 23:32:19 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Thu, 03 Mar 2022 23:32:19 GMT
ENV TERM=xterm
# Thu, 03 Mar 2022 23:39:01 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Thu, 03 Mar 2022 23:39:08 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Thu, 03 Mar 2022 23:39:11 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Thu, 03 Mar 2022 23:39:12 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Thu, 03 Mar 2022 23:39:50 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Thu, 03 Mar 2022 23:39:50 GMT
ENV LANG=en_US.UTF-8
# Thu, 03 Mar 2022 23:39:50 GMT
ENV LANGUAGE=en_US.UTF-8
# Thu, 03 Mar 2022 23:39:50 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 23:39:50 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 03 Mar 2022 23:39:51 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 03 Mar 2022 23:39:51 GMT
ENV JAVA_HOME=/docker-java-home
# Thu, 03 Mar 2022 23:39:51 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Thu, 03 Mar 2022 23:39:51 GMT
ENV JBOSS_HOME=/opt/wildfly
# Thu, 03 Mar 2022 23:39:51 GMT
ENV SILVERPEAS_VERSION=6.2.2
# Thu, 03 Mar 2022 23:39:51 GMT
ENV WILDFLY_VERSION=20.0.1
# Thu, 03 Mar 2022 23:39:52 GMT
LABEL name=Silverpeas 6.2.2 description=Image to install and to run Silverpeas 6.2.2 vendor=Silverpeas version=6.2.2 build=1
# Thu, 03 Mar 2022 23:40:41 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Thu, 03 Mar 2022 23:40:41 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Thu, 03 Mar 2022 23:40:41 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Thu, 03 Mar 2022 23:40:41 GMT
WORKDIR /opt/silverpeas/bin
# Thu, 03 Mar 2022 23:40:41 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Thu, 03 Mar 2022 23:40:41 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Thu, 03 Mar 2022 23:43:15 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Thu, 03 Mar 2022 23:43:18 GMT
EXPOSE 8000 9990
# Thu, 03 Mar 2022 23:43:18 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Thu, 03 Mar 2022 23:43:18 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:7c3b88808835aa80f1ef7f03083c5ae781d0f44e644537cd72de4ce6c5e62e00`  
		Last Modified: Thu, 03 Mar 2022 20:20:44 GMT  
		Size: 28.6 MB (28565751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c468913ed9ca67cb16ab11a0fcfb4ce9c8ba4dfa96b7bceee5da9c77b156d1b8`  
		Last Modified: Thu, 03 Mar 2022 23:56:24 GMT  
		Size: 912.5 MB (912491271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3185928346595d5636736c87cbf1c036ca7a5d98ba0b44a42752eead4c013968`  
		Last Modified: Thu, 03 Mar 2022 23:54:50 GMT  
		Size: 4.0 MB (3994072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c465dd2f9a126532e87c7d001942c30dfd69463a4f2197db9e9012bb5746a4`  
		Last Modified: Thu, 03 Mar 2022 23:54:50 GMT  
		Size: 7.1 MB (7146638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b81543c852334fa9cb7e8018d9fe4962a814ed5ab3555a6603dda4891f3ef2`  
		Last Modified: Thu, 03 Mar 2022 23:54:47 GMT  
		Size: 2.5 MB (2534367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc0ebefe6e61a8a7d5760bb5ce4d8f7a85203a2b976c21480dd9dd2245d8554`  
		Last Modified: Thu, 03 Mar 2022 23:54:46 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8333a36b753ca3617162f3ba5ca939196aac6de8c7673d6af6899e8c14fcc8a`  
		Last Modified: Thu, 03 Mar 2022 23:54:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc872a796e35e4417f0d69147da39651afa8caeb74aeb9da5be53aafc2397f9`  
		Last Modified: Thu, 03 Mar 2022 23:54:59 GMT  
		Size: 196.8 MB (196774063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db45d3424845c626974c6fbbb4bd4a359d5c0d15fba861d5bcc81043a3ce43fd`  
		Last Modified: Thu, 03 Mar 2022 23:54:44 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5155778bd4d8970570975c5c9dfcab031f881ed72d716999fb1c523835fbaf`  
		Last Modified: Thu, 03 Mar 2022 23:54:44 GMT  
		Size: 663.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114222b5de04115cb034ce989a5e37c2186cc870d3f289a98fd50986b0736298`  
		Last Modified: Thu, 03 Mar 2022 23:54:44 GMT  
		Size: 875.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e164e073c4b9897b0e99e39a4bcd7dbef5cd3d5e4f5787e75482f5f5e6ab40c4`  
		Last Modified: Thu, 03 Mar 2022 23:54:44 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85e7a6d695f08129ff9272920cbf34007c01330611bffbd21a4ae243e78ae37`  
		Last Modified: Thu, 03 Mar 2022 23:55:23 GMT  
		Size: 748.0 MB (748021392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
