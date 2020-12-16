<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `silverpeas`

-	[`silverpeas:6.0.2`](#silverpeas602)
-	[`silverpeas:6.1.1`](#silverpeas611)
-	[`silverpeas:latest`](#silverpeaslatest)

## `silverpeas:6.0.2`

```console
$ docker pull silverpeas@sha256:0abb89c8db101b8c4ed7eac7001fc2891434b202516cf5bc728a8e9169cb32c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.0.2` - linux; amd64

```console
$ docker pull silverpeas@sha256:52875b1167eea0e96e6114cb18b324c64b535ba57f826c26cc226e84438decb8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1011722680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b0816407802a649a4e0c74161dffd490e88d7d066ae3a1e8204f5f2488329d9`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Thu, 20 Aug 2020 01:00:50 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Thu, 20 Aug 2020 01:00:50 GMT
ENV TERM=xterm
# Thu, 20 Aug 2020 01:03:10 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Thu, 20 Aug 2020 01:03:12 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Thu, 20 Aug 2020 01:03:14 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Thu, 20 Aug 2020 01:03:15 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Thu, 20 Aug 2020 01:03:17 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Thu, 20 Aug 2020 01:03:17 GMT
ENV LANG=en_US.UTF-8
# Thu, 20 Aug 2020 01:03:18 GMT
ENV LANGUAGE=en_US.UTF-8
# Thu, 20 Aug 2020 01:03:18 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 20 Aug 2020 01:03:19 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 20 Aug 2020 01:03:19 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 20 Aug 2020 01:03:20 GMT
ENV JAVA_HOME=/docker-java-home
# Thu, 20 Aug 2020 01:03:20 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Thu, 20 Aug 2020 01:03:20 GMT
ENV JBOSS_HOME=/opt/wildfly
# Thu, 20 Aug 2020 01:03:20 GMT
ENV SILVERPEAS_VERSION=6.0.2
# Thu, 20 Aug 2020 01:03:20 GMT
ENV WILDFLY_VERSION=10.1.0
# Thu, 20 Aug 2020 01:03:20 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.0.2 build=1
# Thu, 20 Aug 2020 01:03:34 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Thu, 20 Aug 2020 01:03:34 GMT
COPY file:d12fb4c8fc28235c5621533a9ae0d98ba26e3adf1ffc690da4a6118aa71d8190 in /root/.m2/ 
# Thu, 20 Aug 2020 01:03:34 GMT
WORKDIR /opt/silverpeas/bin
# Thu, 20 Aug 2020 01:03:35 GMT
COPY file:31e3db287bacfa9fb086f2ae49169410b9f0fdf4178bf47d0ebe93621aa996e4 in /opt/ 
# Thu, 20 Aug 2020 01:03:35 GMT
COPY file:5d883339e9add47c37406a038c7747cafede9f81436843206bab5bde7da6e2f6 in /opt/silverpeas/configuration/silverpeas/ 
# Thu, 20 Aug 2020 01:06:44 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas assemble   && rm ../log/build-*   && touch .install
# Thu, 20 Aug 2020 01:06:45 GMT
EXPOSE 8000 9990
# Thu, 20 Aug 2020 01:06:45 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/xmlcomponents/workflows]
# Thu, 20 Aug 2020 01:06:46 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31904c357a2c18b6b3722fefba5b7af2d40ea6f0334d61d3562540a5911f56f`  
		Last Modified: Thu, 20 Aug 2020 01:09:06 GMT  
		Size: 206.3 MB (206304801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588eeed35cae42d10c335d44735f0df64657188d2acaeab76dcbb7164bf3795e`  
		Last Modified: Thu, 20 Aug 2020 01:08:30 GMT  
		Size: 4.0 MB (3994029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f0597e47ec76cb9f98c87c39ed819c924585ad960a3facf942a024a5c3ab81`  
		Last Modified: Thu, 20 Aug 2020 01:08:31 GMT  
		Size: 7.1 MB (7146624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a4cd3bfd937ff8bd864270941bbc36b24cdcd41f831b834b4bf5218e1c27b4`  
		Last Modified: Thu, 20 Aug 2020 01:08:29 GMT  
		Size: 845.4 KB (845411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b251ca77bb9f7cb4b21a1262c88f4b070a593af9b522aa32c51cc1c43fad050`  
		Last Modified: Thu, 20 Aug 2020 01:08:28 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66ba30224e189724cdf88f253387ae4077fab04acf1d3b994e93c4ea05931fa`  
		Last Modified: Thu, 20 Aug 2020 01:08:28 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9956a64d4b49f85ef0b2c9e170d9bc396993c1c79c42ae20673d9144e185b3ea`  
		Last Modified: Thu, 20 Aug 2020 01:08:38 GMT  
		Size: 144.3 MB (144284450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f48c831321e9840ea9e910caf26bca3acf99917f4d658f03feee29f43e11bb2`  
		Last Modified: Thu, 20 Aug 2020 01:08:27 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf6f03e9ad1e27dd82ddc56b210fc4a8c96dd2ccd720241ce59df24b2f3bf40`  
		Last Modified: Thu, 20 Aug 2020 01:08:27 GMT  
		Size: 807.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ce2e11be9843f45baea7030e7b9efdcd51ba6f2707783532f182a20eb3c538`  
		Last Modified: Thu, 20 Aug 2020 01:08:27 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9aff22b4e04004dbd5a8f9765db846b251df8346a3c6b2e8076360cf28da04`  
		Last Modified: Thu, 20 Aug 2020 01:09:05 GMT  
		Size: 604.7 MB (604696313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:6.1.1`

**does not exist** (yet?)

## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:fa1d4252b8fc1e48a2987a242d9f0de498e33fc8195610a891ea6bc0a3e622ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:b0093db46dcc70437317858e9e132010aeaf6726001c7d50a78877922fc6c101
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1439789448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46fff63198e279a1ca6f61905ae7e8983e62a08eecfd5bc3079da2eae2f5150c`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Thu, 20 Aug 2020 00:53:43 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Thu, 20 Aug 2020 00:53:43 GMT
ENV TERM=xterm
# Thu, 20 Aug 2020 00:58:12 GMT
RUN apt-get update && apt-get install -y     wget     vim     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Thu, 20 Aug 2020 00:58:16 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Thu, 20 Aug 2020 00:58:19 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Thu, 20 Aug 2020 00:58:19 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Thu, 20 Aug 2020 00:58:22 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Thu, 20 Aug 2020 00:58:22 GMT
ENV LANG=en_US.UTF-8
# Thu, 20 Aug 2020 00:58:22 GMT
ENV LANGUAGE=en_US.UTF-8
# Thu, 20 Aug 2020 00:58:22 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 20 Aug 2020 00:58:23 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 20 Aug 2020 00:58:24 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 20 Aug 2020 00:58:24 GMT
ENV JAVA_HOME=/docker-java-home
# Thu, 20 Aug 2020 00:58:24 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Thu, 20 Aug 2020 00:58:24 GMT
ENV JBOSS_HOME=/opt/wildfly
# Thu, 20 Aug 2020 00:58:25 GMT
ENV SILVERPEAS_VERSION=6.1
# Thu, 20 Aug 2020 00:58:25 GMT
ENV WILDFLY_VERSION=18.0.1
# Thu, 20 Aug 2020 00:58:25 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.1 build=2
# Thu, 20 Aug 2020 00:58:43 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Thu, 20 Aug 2020 00:58:43 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Thu, 20 Aug 2020 00:58:43 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Thu, 20 Aug 2020 00:58:43 GMT
WORKDIR /opt/silverpeas/bin
# Thu, 20 Aug 2020 00:58:43 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Thu, 20 Aug 2020 00:58:44 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Thu, 20 Aug 2020 01:00:33 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && mv ../migrations/db/h2/busCore/up040/alter-table.sql ../migrations/db/h2/busCore/up040/alter_table.sql   && rm ../log/build-*   && touch .install
# Thu, 20 Aug 2020 01:00:34 GMT
EXPOSE 8000 9990
# Thu, 20 Aug 2020 01:00:34 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Thu, 20 Aug 2020 01:00:34 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0547c1440be259f896eb3819c274997eced3ec1fdcee63d38769885c1febec65`  
		Last Modified: Thu, 20 Aug 2020 01:08:22 GMT  
		Size: 491.4 MB (491366826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecb7fd136aade78c0b8bf817f45933bc85640d1d05ab824249c302d062e090b`  
		Last Modified: Thu, 20 Aug 2020 01:07:01 GMT  
		Size: 4.0 MB (3994023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601dbb7d37aba4e9c9926bfa7e101f5dfc42d87a50924c203712e349bde6c360`  
		Last Modified: Thu, 20 Aug 2020 01:07:01 GMT  
		Size: 7.1 MB (7146631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9180922c725f2c83f71900f7e37663b365f78696835798ee12c30cb310265b70`  
		Last Modified: Thu, 20 Aug 2020 01:06:59 GMT  
		Size: 490.7 KB (490688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f34e589c61882e18fc04e3fbbfbcfaa9f30bbfa0bfe074b5cb7858dea3756f`  
		Last Modified: Thu, 20 Aug 2020 01:06:59 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bbcaa2c4dfe36e494d660ed050b588c78c596591ea6aefe478854cba4af9f6`  
		Last Modified: Thu, 20 Aug 2020 01:06:58 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449d37e3c8a1f18e364c660902284a15c1362d48b6aec074eb368eb0197cf066`  
		Last Modified: Thu, 20 Aug 2020 01:07:14 GMT  
		Size: 190.5 MB (190469394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab898ccdef83b2a012fb6e7c72eae8f07461d3e823d63670535abef93880fe7`  
		Last Modified: Thu, 20 Aug 2020 01:06:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205426bbbcad32785bf9ce84a134d99bace685929c58700f95ecf71ef31c14b`  
		Last Modified: Thu, 20 Aug 2020 01:06:57 GMT  
		Size: 663.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34af24e80b2036e74a6c8fc2b848db02113011e6a846a1369654a311bbfbfb2d`  
		Last Modified: Thu, 20 Aug 2020 01:06:57 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a715673f52af1a95d512efe1070ac1c5720f39e9b14086c0e61322d23099930`  
		Last Modified: Thu, 20 Aug 2020 01:06:58 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c237a0cfd8264bab7fcbd8b650ced0fe2c29f1a4b82e89582f2483e658b0cc0`  
		Last Modified: Thu, 20 Aug 2020 01:07:42 GMT  
		Size: 719.6 MB (719582715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
