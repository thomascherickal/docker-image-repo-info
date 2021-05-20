<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `silverpeas`

-	[`silverpeas:6.0.2`](#silverpeas602)
-	[`silverpeas:6.1.3`](#silverpeas613)
-	[`silverpeas:6.2`](#silverpeas62)
-	[`silverpeas:latest`](#silverpeaslatest)

## `silverpeas:6.0.2`

```console
$ docker pull silverpeas@sha256:dc705da42927910d33a3ded43ec8b6f9cb67ea5b991540342f3ed3dad1a138e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.0.2` - linux; amd64

```console
$ docker pull silverpeas@sha256:a9b307e0a64492bab29e895c8dfd1eb31d039068ec7b4ef8cd9c8cfd3c379281
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1014887829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736f677dcba83f696d19a5c343302c7aacb0ca8f55fc055346d550d55412c537`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Wed, 19 May 2021 19:45:15 GMT
ADD file:5dd161b04353d3cbc2b258d66ef3c79a8307faa944953a1c7920a3d97468520c in / 
# Wed, 19 May 2021 19:45:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:45:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 19:45:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:45:19 GMT
CMD ["/bin/bash"]
# Wed, 19 May 2021 22:25:20 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Wed, 19 May 2021 22:25:20 GMT
ENV TERM=xterm
# Wed, 19 May 2021 22:28:57 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Wed, 19 May 2021 22:29:02 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Wed, 19 May 2021 22:29:06 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Wed, 19 May 2021 22:29:06 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Wed, 19 May 2021 22:29:09 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Wed, 19 May 2021 22:29:09 GMT
ENV LANG=en_US.UTF-8
# Wed, 19 May 2021 22:29:09 GMT
ENV LANGUAGE=en_US.UTF-8
# Wed, 19 May 2021 22:29:10 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 19 May 2021 22:29:11 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 19 May 2021 22:29:12 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 19 May 2021 22:29:12 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 19 May 2021 22:29:12 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Wed, 19 May 2021 22:29:12 GMT
ENV JBOSS_HOME=/opt/wildfly
# Wed, 19 May 2021 22:29:13 GMT
ENV SILVERPEAS_VERSION=6.0.2
# Wed, 19 May 2021 22:29:13 GMT
ENV WILDFLY_VERSION=10.1.0
# Wed, 19 May 2021 22:29:13 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.0.2 build=1
# Wed, 19 May 2021 22:29:29 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Wed, 19 May 2021 22:29:29 GMT
COPY file:d12fb4c8fc28235c5621533a9ae0d98ba26e3adf1ffc690da4a6118aa71d8190 in /root/.m2/ 
# Wed, 19 May 2021 22:29:29 GMT
WORKDIR /opt/silverpeas/bin
# Wed, 19 May 2021 22:29:30 GMT
COPY file:31e3db287bacfa9fb086f2ae49169410b9f0fdf4178bf47d0ebe93621aa996e4 in /opt/ 
# Wed, 19 May 2021 22:29:30 GMT
COPY file:5d883339e9add47c37406a038c7747cafede9f81436843206bab5bde7da6e2f6 in /opt/silverpeas/configuration/silverpeas/ 
# Wed, 19 May 2021 22:36:00 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas assemble   && rm ../log/build-*   && touch .install
# Wed, 19 May 2021 22:36:03 GMT
EXPOSE 8000 9990
# Wed, 19 May 2021 22:36:03 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/xmlcomponents/workflows]
# Wed, 19 May 2021 22:36:03 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:80bce60046fa9e5ccbe54c9bd4bfa3f379ce7bc43bed493ae92389050de04024`  
		Last Modified: Thu, 29 Apr 2021 15:24:23 GMT  
		Size: 46.5 MB (46461779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a738a1554069bc9050c0a60b57fc93e98069e59822677a483cc74cafaf2bf7`  
		Last Modified: Wed, 19 May 2021 19:46:37 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19cf0706c6229033d11dbf952b3eb96ad70e1f32527960aeb3c83ad86f16551`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4cdd6c27d1f17cf5ff350e76b7efe80aceff4dc99fd518065bf048abd6494a`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9e8c74489f8fbab8fd6979741dc4382a47d88d69c6f317517cb4ea21a4be5d`  
		Last Modified: Wed, 19 May 2021 22:38:29 GMT  
		Size: 207.5 MB (207456337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e00dcf53094b0200a972b4b3b2bd194d2cb163ec10f88750e8b089dd8d6e1bd`  
		Last Modified: Wed, 19 May 2021 22:38:00 GMT  
		Size: 4.0 MB (3994089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bcf1cf596b3a5ec430f1d8c090507998ff927bc96432d970a8c1a21055f07e`  
		Last Modified: Wed, 19 May 2021 22:38:02 GMT  
		Size: 7.1 MB (7146641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca617a720e4fb1e05865e41188ded788e5c3cb8bc210bbc8427068ae54697c8e`  
		Last Modified: Wed, 19 May 2021 22:37:57 GMT  
		Size: 845.4 KB (845400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a510606b02df8381d7d36181796f9ebc845dc683722e199dc9c745d7fd684aa6`  
		Last Modified: Wed, 19 May 2021 22:37:57 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd184b2ac1e9f924256ae2593faddbf8dae7644b0dc3ff24a6d34fc62418034f`  
		Last Modified: Wed, 19 May 2021 22:37:56 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f99dcfb050aa9f04221a3a50b28a587e4e3ae35f011e1be003ef490639a459`  
		Last Modified: Wed, 19 May 2021 22:38:04 GMT  
		Size: 144.3 MB (144284757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a711a2db3c5b145d6e2d117a1bcaee9d195cb7aacc0f719833824c2ca950ef`  
		Last Modified: Wed, 19 May 2021 22:37:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25952ba6a9acd9fc090ef7134f64dec45e4c635472afedf969309517e786b4e`  
		Last Modified: Wed, 19 May 2021 22:37:54 GMT  
		Size: 806.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f005f89301ff113cb10b61df19706a3633909eb7d2b9c1572a21b230d55c5e`  
		Last Modified: Wed, 19 May 2021 22:37:54 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fb151a6b83b983e0dbcb138388c7fd4427c3200b75168300fd42d75f79e8c`  
		Last Modified: Wed, 19 May 2021 22:38:28 GMT  
		Size: 604.7 MB (604695313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:6.1.3`

```console
$ docker pull silverpeas@sha256:aa1f9f4f36e27f98dbf328695236184136baf64456fcf0803c3be9a4f90e7b9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.1.3` - linux; amd64

```console
$ docker pull silverpeas@sha256:0864a88b1e5ccc5babd116cee3cf257ca96a483735467a4c806e4814396df30d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1426503842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc56e1f265812749c5b27084949ccc4b21ab6bdf107bd1b09a08cac38eeac7ba`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Wed, 19 May 2021 19:44:30 GMT
ADD file:e05689b5b0d51a2316f8a87b1a9d6cbf90d98b19a424dbb924ee3d0b1cc17bfc in / 
# Wed, 19 May 2021 19:44:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:44:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 19:44:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:44:33 GMT
CMD ["/bin/bash"]
# Wed, 19 May 2021 22:16:52 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Wed, 19 May 2021 22:16:53 GMT
ENV TERM=xterm
# Wed, 19 May 2021 22:21:37 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Wed, 19 May 2021 22:21:42 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Wed, 19 May 2021 22:21:47 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Wed, 19 May 2021 22:21:47 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Wed, 19 May 2021 22:21:50 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Wed, 19 May 2021 22:21:50 GMT
ENV LANG=en_US.UTF-8
# Wed, 19 May 2021 22:21:50 GMT
ENV LANGUAGE=en_US.UTF-8
# Wed, 19 May 2021 22:21:50 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 19 May 2021 22:21:51 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 19 May 2021 22:21:52 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 19 May 2021 22:21:52 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 19 May 2021 22:21:53 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Wed, 19 May 2021 22:21:53 GMT
ENV JBOSS_HOME=/opt/wildfly
# Wed, 19 May 2021 22:21:53 GMT
ENV SILVERPEAS_VERSION=6.1.3
# Wed, 19 May 2021 22:21:53 GMT
ENV WILDFLY_VERSION=18.0.1
# Wed, 19 May 2021 22:21:53 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.1.3 build=1
# Wed, 19 May 2021 22:23:06 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Wed, 19 May 2021 22:23:06 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Wed, 19 May 2021 22:23:06 GMT
WORKDIR /opt/silverpeas/bin
# Wed, 19 May 2021 22:23:07 GMT
COPY file:bd0a4d5e9017df7c7d4b9ba1011c737b2e2fcbe0966662e3315fabb5498b8aa3 in /opt/ 
# Wed, 19 May 2021 22:23:07 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Wed, 19 May 2021 22:25:10 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas construct   && rm ../log/build-*   && touch .install
# Wed, 19 May 2021 22:25:13 GMT
EXPOSE 8000 9990
# Wed, 19 May 2021 22:25:13 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Wed, 19 May 2021 22:25:13 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:4bbfd2c87b7524455f144a03bf387c88b6d4200e5e0df9139a9d5e79110f89ca`  
		Last Modified: Thu, 13 May 2021 14:54:04 GMT  
		Size: 26.7 MB (26696304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e110be24e168b42c1a2ddbc4a476a217b73cccdba69cdcb212b812a88f5726`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889a7173dcfeb409f9d88054a97ab2445f5a799a823f719a5573365ee3662b6f`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614a587cb631cd04844f151c7de5d8bf9033ed15904e2d8ef531f86a3a2e8d5c`  
		Last Modified: Wed, 19 May 2021 22:37:41 GMT  
		Size: 481.4 MB (481419381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9f77fae368abcb0def20e9fd4249d44d450b6700367afb3b53fe40648e5107`  
		Last Modified: Wed, 19 May 2021 22:36:35 GMT  
		Size: 4.0 MB (3994089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6626bece258285763d2e6b102085b75a7596c626471ec1c3cfdc318605afecc0`  
		Last Modified: Wed, 19 May 2021 22:36:36 GMT  
		Size: 7.1 MB (7146666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecb7e873c1ecc6078a066b8f03b840b9789388f6c3a828fd1b981eb469bca63`  
		Last Modified: Wed, 19 May 2021 22:36:32 GMT  
		Size: 490.7 KB (490685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e71e950733de66996d035f5fae64d745837e39685c3db031ccead2aa2ec2a0d`  
		Last Modified: Wed, 19 May 2021 22:36:31 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a60f20d9aeb20560ce4dd9558d961a6682e4f14b59242ea2fc5958cb1df60f`  
		Last Modified: Wed, 19 May 2021 22:36:31 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3756a25114bfd1fa1c9e6d5ab9a34c45fa8119cc1e94fd01bb662b666d009a2f`  
		Last Modified: Wed, 19 May 2021 22:36:42 GMT  
		Size: 190.5 MB (190469427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae58f8b74d6c5c1770b104b9c3949becca4871168d884f13100e55e6ac8a5f8`  
		Last Modified: Wed, 19 May 2021 22:36:29 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422571ceba8a10f2521823bd52272831f47c734e59a5dd262eacc443585b619`  
		Last Modified: Wed, 19 May 2021 22:36:29 GMT  
		Size: 762.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69f2ab898b816627d31b8d800ef22deca4af50eabf9d593490f54010540fd29`  
		Last Modified: Wed, 19 May 2021 22:36:29 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf446e4b6872d0c96ab11fbca75a9accc1fbcdb25231a076e84125e552e12bfb`  
		Last Modified: Wed, 19 May 2021 22:37:08 GMT  
		Size: 716.3 MB (716284325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:6.2`

```console
$ docker pull silverpeas@sha256:0592fa1d8760aeef620323c09718ed76d5fabc86e0d9147c938a58d638c45c18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.2` - linux; amd64

```console
$ docker pull silverpeas@sha256:59d60b04305cb885dad7f8c933b329e8ee8551be4d8d624c67b6111602603244
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1867239280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a6645b33a105f809dd625bb78592e19cbbf1717910956a30f19c9d75cf07776`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:18:49 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Sat, 24 Apr 2021 02:18:49 GMT
ENV TERM=xterm
# Sat, 24 Apr 2021 02:27:01 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Sat, 24 Apr 2021 02:27:07 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Sat, 24 Apr 2021 02:27:11 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Sat, 24 Apr 2021 02:27:11 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Sat, 24 Apr 2021 02:27:48 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Sat, 24 Apr 2021 02:27:48 GMT
ENV LANG=en_US.UTF-8
# Sat, 24 Apr 2021 02:27:48 GMT
ENV LANGUAGE=en_US.UTF-8
# Sat, 24 Apr 2021 02:27:49 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 24 Apr 2021 02:27:50 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 24 Apr 2021 02:27:50 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 24 Apr 2021 02:27:51 GMT
ENV JAVA_HOME=/docker-java-home
# Sat, 24 Apr 2021 02:27:51 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Sat, 24 Apr 2021 02:27:51 GMT
ENV JBOSS_HOME=/opt/wildfly
# Sat, 24 Apr 2021 02:27:51 GMT
ENV SILVERPEAS_VERSION=6.2
# Sat, 24 Apr 2021 02:27:51 GMT
ENV WILDFLY_VERSION=20.0.1
# Sat, 24 Apr 2021 02:27:52 GMT
LABEL name=Silverpeas 6.2 description=Image to install and to run Silverpeas 6.2 vendor=Silverpeas version=6.2 build=1
# Sat, 24 Apr 2021 02:28:01 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Sat, 24 Apr 2021 02:28:02 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Sat, 24 Apr 2021 02:28:02 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Sat, 24 Apr 2021 02:28:02 GMT
WORKDIR /opt/silverpeas/bin
# Sat, 24 Apr 2021 02:28:03 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Sat, 24 Apr 2021 02:28:03 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Sat, 24 Apr 2021 02:29:57 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Sat, 24 Apr 2021 02:30:00 GMT
EXPOSE 8000 9990
# Sat, 24 Apr 2021 02:30:00 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Sat, 24 Apr 2021 02:30:00 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6aae5e3e8e5aff7a9423f55046117c45048b8e106c060e05118a408a1271182`  
		Last Modified: Sat, 24 Apr 2021 02:51:11 GMT  
		Size: 906.3 MB (906293062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866924950606a552ae78739f70ca64b46db27e0e590bf99dd3a15068a6433760`  
		Last Modified: Sat, 24 Apr 2021 02:49:30 GMT  
		Size: 4.0 MB (3994081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69672c8fe71b653158499ced9212e53ffac2d810216da0a0a10d01a0b24b097e`  
		Last Modified: Sat, 24 Apr 2021 02:49:30 GMT  
		Size: 7.1 MB (7146661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537e0d2145c71511aa3574b66630e42d310911a5d5e788cd9a4da6ca91c949a6`  
		Last Modified: Sat, 24 Apr 2021 02:49:27 GMT  
		Size: 2.5 MB (2534359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5adb452e7e30a76d1445083277cc4a6a4528bc464ffd9e6ce8d6a8fe2d17985`  
		Last Modified: Sat, 24 Apr 2021 02:49:26 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a076f3df17a4e6e4a31b77863a051f6c859efb75a4aa437f30faae7ec7a83a`  
		Last Modified: Sat, 24 Apr 2021 02:49:26 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5900b7497466b60ca1af4bd5d9de76ff43e9c7207bf243f5840151f4934d185`  
		Last Modified: Sat, 24 Apr 2021 02:49:40 GMT  
		Size: 196.8 MB (196774017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95e4d00fd96bb5269c4ad07b136c1d069672939a6b19a5e6d078cc12224cf47`  
		Last Modified: Sat, 24 Apr 2021 02:49:23 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f63ceaaba965788920b5f74f7d914a7c8911dd77cb536dccf99c6889df62a3e`  
		Last Modified: Sat, 24 Apr 2021 02:49:23 GMT  
		Size: 659.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df70237302aefc53307802c9f74ec21bc97fd25c21d73cddcb073bcb51de26`  
		Last Modified: Sat, 24 Apr 2021 02:49:23 GMT  
		Size: 874.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1e7ec01847160cbdf358cb0cb7713b1657ea17e494523cdf9d7534b04c4739`  
		Last Modified: Sat, 24 Apr 2021 02:49:23 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b27db0d3a0d8ba445fac0041aeafa0ecf26b11099725a2083bbca2cc5dc0dc`  
		Last Modified: Sat, 24 Apr 2021 02:50:02 GMT  
		Size: 722.0 MB (721953745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:0592fa1d8760aeef620323c09718ed76d5fabc86e0d9147c938a58d638c45c18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:59d60b04305cb885dad7f8c933b329e8ee8551be4d8d624c67b6111602603244
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1867239280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a6645b33a105f809dd625bb78592e19cbbf1717910956a30f19c9d75cf07776`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:18:49 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Sat, 24 Apr 2021 02:18:49 GMT
ENV TERM=xterm
# Sat, 24 Apr 2021 02:27:01 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Sat, 24 Apr 2021 02:27:07 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Sat, 24 Apr 2021 02:27:11 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Sat, 24 Apr 2021 02:27:11 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Sat, 24 Apr 2021 02:27:48 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Sat, 24 Apr 2021 02:27:48 GMT
ENV LANG=en_US.UTF-8
# Sat, 24 Apr 2021 02:27:48 GMT
ENV LANGUAGE=en_US.UTF-8
# Sat, 24 Apr 2021 02:27:49 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 24 Apr 2021 02:27:50 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 24 Apr 2021 02:27:50 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 24 Apr 2021 02:27:51 GMT
ENV JAVA_HOME=/docker-java-home
# Sat, 24 Apr 2021 02:27:51 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Sat, 24 Apr 2021 02:27:51 GMT
ENV JBOSS_HOME=/opt/wildfly
# Sat, 24 Apr 2021 02:27:51 GMT
ENV SILVERPEAS_VERSION=6.2
# Sat, 24 Apr 2021 02:27:51 GMT
ENV WILDFLY_VERSION=20.0.1
# Sat, 24 Apr 2021 02:27:52 GMT
LABEL name=Silverpeas 6.2 description=Image to install and to run Silverpeas 6.2 vendor=Silverpeas version=6.2 build=1
# Sat, 24 Apr 2021 02:28:01 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Sat, 24 Apr 2021 02:28:02 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Sat, 24 Apr 2021 02:28:02 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Sat, 24 Apr 2021 02:28:02 GMT
WORKDIR /opt/silverpeas/bin
# Sat, 24 Apr 2021 02:28:03 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Sat, 24 Apr 2021 02:28:03 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Sat, 24 Apr 2021 02:29:57 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Sat, 24 Apr 2021 02:30:00 GMT
EXPOSE 8000 9990
# Sat, 24 Apr 2021 02:30:00 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Sat, 24 Apr 2021 02:30:00 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6aae5e3e8e5aff7a9423f55046117c45048b8e106c060e05118a408a1271182`  
		Last Modified: Sat, 24 Apr 2021 02:51:11 GMT  
		Size: 906.3 MB (906293062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866924950606a552ae78739f70ca64b46db27e0e590bf99dd3a15068a6433760`  
		Last Modified: Sat, 24 Apr 2021 02:49:30 GMT  
		Size: 4.0 MB (3994081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69672c8fe71b653158499ced9212e53ffac2d810216da0a0a10d01a0b24b097e`  
		Last Modified: Sat, 24 Apr 2021 02:49:30 GMT  
		Size: 7.1 MB (7146661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537e0d2145c71511aa3574b66630e42d310911a5d5e788cd9a4da6ca91c949a6`  
		Last Modified: Sat, 24 Apr 2021 02:49:27 GMT  
		Size: 2.5 MB (2534359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5adb452e7e30a76d1445083277cc4a6a4528bc464ffd9e6ce8d6a8fe2d17985`  
		Last Modified: Sat, 24 Apr 2021 02:49:26 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a076f3df17a4e6e4a31b77863a051f6c859efb75a4aa437f30faae7ec7a83a`  
		Last Modified: Sat, 24 Apr 2021 02:49:26 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5900b7497466b60ca1af4bd5d9de76ff43e9c7207bf243f5840151f4934d185`  
		Last Modified: Sat, 24 Apr 2021 02:49:40 GMT  
		Size: 196.8 MB (196774017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95e4d00fd96bb5269c4ad07b136c1d069672939a6b19a5e6d078cc12224cf47`  
		Last Modified: Sat, 24 Apr 2021 02:49:23 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f63ceaaba965788920b5f74f7d914a7c8911dd77cb536dccf99c6889df62a3e`  
		Last Modified: Sat, 24 Apr 2021 02:49:23 GMT  
		Size: 659.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df70237302aefc53307802c9f74ec21bc97fd25c21d73cddcb073bcb51de26`  
		Last Modified: Sat, 24 Apr 2021 02:49:23 GMT  
		Size: 874.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1e7ec01847160cbdf358cb0cb7713b1657ea17e494523cdf9d7534b04c4739`  
		Last Modified: Sat, 24 Apr 2021 02:49:23 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b27db0d3a0d8ba445fac0041aeafa0ecf26b11099725a2083bbca2cc5dc0dc`  
		Last Modified: Sat, 24 Apr 2021 02:50:02 GMT  
		Size: 722.0 MB (721953745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
