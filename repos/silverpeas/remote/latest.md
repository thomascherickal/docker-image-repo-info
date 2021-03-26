## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:fb8bc59e9f7f658bfeb886214eb7854f97075c057219f0fb88a52fbc63ab2f5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:cf57d4919d8914aa326c92ca096fe1849e1eff79e9d4180bc0a897ee1b503efb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1865914414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:404fa17711392b832a67e358457df29a414dccc819858ca5ef2d7a8fb6d584b8`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:08 GMT
ADD file:a8d2f02fbaddf8cec8e4da320cd03c06435f395e9d454f69954efe422eb6e1ba in / 
# Thu, 25 Mar 2021 22:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:11 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 15:35:23 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Fri, 26 Mar 2021 15:35:23 GMT
ENV TERM=xterm
# Fri, 26 Mar 2021 15:46:07 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Fri, 26 Mar 2021 15:46:14 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Fri, 26 Mar 2021 15:46:19 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Fri, 26 Mar 2021 15:46:19 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Fri, 26 Mar 2021 15:47:15 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Fri, 26 Mar 2021 15:47:16 GMT
ENV LANG=en_US.UTF-8
# Fri, 26 Mar 2021 15:47:16 GMT
ENV LANGUAGE=en_US.UTF-8
# Fri, 26 Mar 2021 15:47:16 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 26 Mar 2021 15:47:18 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 26 Mar 2021 15:47:20 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 26 Mar 2021 15:47:20 GMT
ENV JAVA_HOME=/docker-java-home
# Fri, 26 Mar 2021 15:47:20 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Fri, 26 Mar 2021 15:47:21 GMT
ENV JBOSS_HOME=/opt/wildfly
# Fri, 26 Mar 2021 15:47:21 GMT
ENV SILVERPEAS_VERSION=6.2
# Fri, 26 Mar 2021 15:47:21 GMT
ENV WILDFLY_VERSION=20.0.1
# Fri, 26 Mar 2021 15:47:21 GMT
LABEL name=Silverpeas 6.2 description=Image to install and to run Silverpeas 6.2 vendor=Silverpeas version=6.2 build=1
# Fri, 26 Mar 2021 15:48:27 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Fri, 26 Mar 2021 15:48:28 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Fri, 26 Mar 2021 15:48:29 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Fri, 26 Mar 2021 15:48:29 GMT
WORKDIR /opt/silverpeas/bin
# Fri, 26 Mar 2021 15:48:30 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Fri, 26 Mar 2021 15:48:30 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Fri, 26 Mar 2021 15:50:40 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Fri, 26 Mar 2021 15:50:44 GMT
EXPOSE 8000 9990
# Fri, 26 Mar 2021 15:50:44 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Fri, 26 Mar 2021 15:50:45 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:04a5f4cda3eea2313a61a2f72208342a57ea36a9326dff54f4f26ed47d145c7c`  
		Last Modified: Thu, 25 Mar 2021 22:34:46 GMT  
		Size: 28.6 MB (28569428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff496a88c8ed9b745dab2f00bfbd9013c6d1db198442a6a8683998a29a85458a`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce83f459fe7e0bf459d0c222ef3b2ca4d9911f6b0f9aae02c2120561b54ca18`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3cd2d1e7eb70d5ab2356319f32d652edf5660d30d302cbe454745d615a4f46`  
		Last Modified: Fri, 26 Mar 2021 16:17:06 GMT  
		Size: 904.9 MB (904942322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5001dc0916128fb1522a96b2d4ed10002d211ed13acbaf48e70e752753218b03`  
		Last Modified: Fri, 26 Mar 2021 16:14:14 GMT  
		Size: 4.0 MB (3994068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5a49abd751c663b62cf9e0992adfa2a5d3f730d7de691357cdc3f3f1dd3f29`  
		Last Modified: Fri, 26 Mar 2021 16:14:15 GMT  
		Size: 7.1 MB (7146661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07e0326a8a95c3670357921e49d67bf0e703b295c8c758d7290181232e7e880`  
		Last Modified: Fri, 26 Mar 2021 16:14:12 GMT  
		Size: 2.5 MB (2534367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a8857d53e6025d0a0a856606ad416f76b74220d76a75e3ab49c6c0572fbb3f`  
		Last Modified: Fri, 26 Mar 2021 16:14:09 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7fa5d83e08320ac5f2cb281705fff301ba20eed162eaf032518f7c729a6a79`  
		Last Modified: Fri, 26 Mar 2021 16:14:09 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8ebea65cd9beb055bb306744fad7cd0843270233095675b6a8e2b1502bd2eb`  
		Last Modified: Fri, 26 Mar 2021 16:14:38 GMT  
		Size: 196.8 MB (196774104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26589671347dbcbe3a1fb90dcd24b720e5e3c3209cdfea1ea4eae3ee0b37946`  
		Last Modified: Fri, 26 Mar 2021 16:14:06 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63b71dd09281dcb4635b3f7719883695fc519c0296c6e3f2c6f82aff30871b4`  
		Last Modified: Fri, 26 Mar 2021 16:14:06 GMT  
		Size: 663.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83f4f3e46770b21beea95dc354e02e759b0c89e0821b2033b3e235cfc5a9ab3`  
		Last Modified: Fri, 26 Mar 2021 16:14:06 GMT  
		Size: 878.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45898b22d00c28cd91e38a50fb6c4e565bbe3a8a475975bafdc06c7e3fa5bae8`  
		Last Modified: Fri, 26 Mar 2021 16:14:06 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af825a96b33b034580967da4d76ac1543c72195b413eb533274b46a920b179ee`  
		Last Modified: Fri, 26 Mar 2021 16:15:26 GMT  
		Size: 721.9 MB (721949723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
