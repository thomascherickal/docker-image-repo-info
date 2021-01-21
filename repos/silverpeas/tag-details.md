<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `silverpeas`

-	[`silverpeas:6.0.2`](#silverpeas602)
-	[`silverpeas:6.1.1`](#silverpeas611)
-	[`silverpeas:latest`](#silverpeaslatest)

## `silverpeas:6.0.2`

```console
$ docker pull silverpeas@sha256:958ec57365c19a0aa4cd779fc209a529d5dcbcf631c415265391471b1826f2c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.0.2` - linux; amd64

```console
$ docker pull silverpeas@sha256:418139f1b60235429e59466553b9c650fd3fd23ec6e9767efcab4cd03e3782f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1014322051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f35f44045b83564556ad9e5b051a6b988f0c8d7151a21b80cfe39d95fe3e804`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:41:19 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Thu, 21 Jan 2021 10:41:19 GMT
ENV TERM=xterm
# Thu, 21 Jan 2021 10:43:24 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Thu, 21 Jan 2021 10:43:27 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Thu, 21 Jan 2021 10:43:30 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Thu, 21 Jan 2021 10:43:31 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Thu, 21 Jan 2021 10:43:34 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Thu, 21 Jan 2021 10:43:34 GMT
ENV LANG=en_US.UTF-8
# Thu, 21 Jan 2021 10:43:34 GMT
ENV LANGUAGE=en_US.UTF-8
# Thu, 21 Jan 2021 10:43:34 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 21 Jan 2021 10:43:35 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 21 Jan 2021 10:43:36 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 21 Jan 2021 10:43:36 GMT
ENV JAVA_HOME=/docker-java-home
# Thu, 21 Jan 2021 10:43:36 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Thu, 21 Jan 2021 10:43:37 GMT
ENV JBOSS_HOME=/opt/wildfly
# Thu, 21 Jan 2021 10:43:37 GMT
ENV SILVERPEAS_VERSION=6.0.2
# Thu, 21 Jan 2021 10:43:37 GMT
ENV WILDFLY_VERSION=10.1.0
# Thu, 21 Jan 2021 10:43:37 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.0.2 build=1
# Thu, 21 Jan 2021 10:43:46 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Thu, 21 Jan 2021 10:43:46 GMT
COPY file:d12fb4c8fc28235c5621533a9ae0d98ba26e3adf1ffc690da4a6118aa71d8190 in /root/.m2/ 
# Thu, 21 Jan 2021 10:43:46 GMT
WORKDIR /opt/silverpeas/bin
# Thu, 21 Jan 2021 10:43:46 GMT
COPY file:31e3db287bacfa9fb086f2ae49169410b9f0fdf4178bf47d0ebe93621aa996e4 in /opt/ 
# Thu, 21 Jan 2021 10:43:47 GMT
COPY file:5d883339e9add47c37406a038c7747cafede9f81436843206bab5bde7da6e2f6 in /opt/silverpeas/configuration/silverpeas/ 
# Thu, 21 Jan 2021 10:48:22 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas assemble   && rm ../log/build-*   && touch .install
# Thu, 21 Jan 2021 10:48:23 GMT
EXPOSE 8000 9990
# Thu, 21 Jan 2021 10:48:23 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/xmlcomponents/workflows]
# Thu, 21 Jan 2021 10:48:24 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485d6cc6deeb0e6aaff53d82980aff7608d697d87a1ffe69cf09996f7ad9c2e1`  
		Last Modified: Thu, 21 Jan 2021 10:51:16 GMT  
		Size: 207.4 MB (207389840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d65be3921226b9d9a5408d2e7dea1fd6503f1fc97e312facffd7b06bfd41226`  
		Last Modified: Thu, 21 Jan 2021 10:50:39 GMT  
		Size: 4.0 MB (3994034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d9ff6825183c27656c9e2ae60ced8a2cf7df094b0824992f45538b77dd8545`  
		Last Modified: Thu, 21 Jan 2021 10:50:39 GMT  
		Size: 7.1 MB (7146616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d2f0e81b1afd6c80f57f3f9ed6d71cadf0da0046715948bff62ddbfc4e6828`  
		Last Modified: Thu, 21 Jan 2021 10:50:38 GMT  
		Size: 845.4 KB (845413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea9fe0e5091cf32faddec0d40906e6768f651680e42ef718d92478067935571`  
		Last Modified: Thu, 21 Jan 2021 10:50:35 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d69ab684f108a7e4a189f9bd219dcff77294a7f6e9593b2beee6f43b17d423`  
		Last Modified: Thu, 21 Jan 2021 10:50:35 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991b03265f7d07e4af469c173551d9fb53287a53a77a08821e6159a0e98df63f`  
		Last Modified: Thu, 21 Jan 2021 10:50:46 GMT  
		Size: 144.3 MB (144284541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a5baa6ccc140c0d7705472ecddd0a4db73f6c4c994e0ea08f25b57e077dd36`  
		Last Modified: Thu, 21 Jan 2021 10:50:34 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2293c265ff151f607fc523cc2e490378ad978a3f436c51e77b558da5bf8cfce`  
		Last Modified: Thu, 21 Jan 2021 10:50:34 GMT  
		Size: 808.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3091881f974323e6093ac70761f000f0ff7892e05df79448bc29791848086f3`  
		Last Modified: Thu, 21 Jan 2021 10:50:34 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9079e76782c1dafcd2f9294150fab265a8e7c2f44b2cd61844586190fade8686`  
		Last Modified: Thu, 21 Jan 2021 10:51:13 GMT  
		Size: 604.7 MB (604695746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:6.1.1`

```console
$ docker pull silverpeas@sha256:ba1947ff8db30f4d7b976d43ddca31fbaf0496d1696c97b77ce4a34601104a79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.1.1` - linux; amd64

```console
$ docker pull silverpeas@sha256:21327cc912606042af18e45be20ed9f4f99c90957f7a815fb7334d1f8c9f7c37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1427263054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1e9ff528b85576f6f6d9dc034d7e0dff3796db5e8f5ae65aac1f0a126f6a02`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:32:26 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Thu, 21 Jan 2021 10:32:26 GMT
ENV TERM=xterm
# Thu, 21 Jan 2021 10:37:06 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Thu, 21 Jan 2021 10:37:11 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Thu, 21 Jan 2021 10:37:15 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Thu, 21 Jan 2021 10:37:15 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Thu, 21 Jan 2021 10:37:18 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Thu, 21 Jan 2021 10:37:18 GMT
ENV LANG=en_US.UTF-8
# Thu, 21 Jan 2021 10:37:19 GMT
ENV LANGUAGE=en_US.UTF-8
# Thu, 21 Jan 2021 10:37:19 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 21 Jan 2021 10:37:20 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 21 Jan 2021 10:37:21 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 21 Jan 2021 10:37:21 GMT
ENV JAVA_HOME=/docker-java-home
# Thu, 21 Jan 2021 10:37:21 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Thu, 21 Jan 2021 10:37:21 GMT
ENV JBOSS_HOME=/opt/wildfly
# Thu, 21 Jan 2021 10:37:22 GMT
ENV SILVERPEAS_VERSION=6.1.1
# Thu, 21 Jan 2021 10:37:22 GMT
ENV WILDFLY_VERSION=18.0.1
# Thu, 21 Jan 2021 10:37:22 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.1.1 build=1
# Thu, 21 Jan 2021 10:38:56 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Thu, 21 Jan 2021 10:38:56 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Thu, 21 Jan 2021 10:38:56 GMT
WORKDIR /opt/silverpeas/bin
# Thu, 21 Jan 2021 10:38:56 GMT
COPY file:bd0a4d5e9017df7c7d4b9ba1011c737b2e2fcbe0966662e3315fabb5498b8aa3 in /opt/ 
# Thu, 21 Jan 2021 10:38:57 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Thu, 21 Jan 2021 10:41:02 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas construct   && rm ../log/build-*   && touch .install
# Thu, 21 Jan 2021 10:41:02 GMT
EXPOSE 8000 9990
# Thu, 21 Jan 2021 10:41:03 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Thu, 21 Jan 2021 10:41:03 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453ffa30280ef058ed197c390928409b9c7b71a5ab28429d75b2307a47f291b2`  
		Last Modified: Thu, 21 Jan 2021 10:50:17 GMT  
		Size: 482.2 MB (482188669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef987cc50d56d036e369823e849cfb4cb41adf67656e68bc54e53bd7a803e91`  
		Last Modified: Thu, 21 Jan 2021 10:48:55 GMT  
		Size: 4.0 MB (3994026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81079500a3c91140f06b7fbfcc1664569e984a40ecd4e1f6a1983060dfa9a694`  
		Last Modified: Thu, 21 Jan 2021 10:48:54 GMT  
		Size: 7.1 MB (7146628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe187cdb5e1a91b85d3c5bfd66580416a489563d1097ea796dcd082d9189338`  
		Last Modified: Thu, 21 Jan 2021 10:48:51 GMT  
		Size: 490.7 KB (490686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f5f5835de95fd95d76c71aa24e82cd51f100786ff1565a271f93290bc4896c`  
		Last Modified: Thu, 21 Jan 2021 10:48:50 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6169ff8b6b1aaed1447ec19cbcadfe4784a64261c0a8fd4bcb2a1f251d17120`  
		Last Modified: Thu, 21 Jan 2021 10:48:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8066b4330a1965273f00ef9e2246af7c3dd96b7aa28175fa0355791292281518`  
		Last Modified: Thu, 21 Jan 2021 10:49:09 GMT  
		Size: 190.5 MB (190469093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea062f3d89f89c824c360489241820725f7dd8f60c1834d42ed9306b48350d9`  
		Last Modified: Thu, 21 Jan 2021 10:48:49 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d2ca84793979f4ae2a5ab68e164a971879a9ee960ac5797cf31744f46c75ce`  
		Last Modified: Thu, 21 Jan 2021 10:48:49 GMT  
		Size: 759.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a39df8a7f54f3086dbb92c7a3352a3099b1fe88c7af5c4548211b7c8f1ff83`  
		Last Modified: Thu, 21 Jan 2021 10:48:49 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0324f4ddb35888a5fbc04a06467ecc6066fc4092cc1b31ae0273c4c915e28129`  
		Last Modified: Thu, 21 Jan 2021 10:49:45 GMT  
		Size: 716.3 MB (716261302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:ba1947ff8db30f4d7b976d43ddca31fbaf0496d1696c97b77ce4a34601104a79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:21327cc912606042af18e45be20ed9f4f99c90957f7a815fb7334d1f8c9f7c37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1427263054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1e9ff528b85576f6f6d9dc034d7e0dff3796db5e8f5ae65aac1f0a126f6a02`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:32:26 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Thu, 21 Jan 2021 10:32:26 GMT
ENV TERM=xterm
# Thu, 21 Jan 2021 10:37:06 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Thu, 21 Jan 2021 10:37:11 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Thu, 21 Jan 2021 10:37:15 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Thu, 21 Jan 2021 10:37:15 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Thu, 21 Jan 2021 10:37:18 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Thu, 21 Jan 2021 10:37:18 GMT
ENV LANG=en_US.UTF-8
# Thu, 21 Jan 2021 10:37:19 GMT
ENV LANGUAGE=en_US.UTF-8
# Thu, 21 Jan 2021 10:37:19 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 21 Jan 2021 10:37:20 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 21 Jan 2021 10:37:21 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 21 Jan 2021 10:37:21 GMT
ENV JAVA_HOME=/docker-java-home
# Thu, 21 Jan 2021 10:37:21 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Thu, 21 Jan 2021 10:37:21 GMT
ENV JBOSS_HOME=/opt/wildfly
# Thu, 21 Jan 2021 10:37:22 GMT
ENV SILVERPEAS_VERSION=6.1.1
# Thu, 21 Jan 2021 10:37:22 GMT
ENV WILDFLY_VERSION=18.0.1
# Thu, 21 Jan 2021 10:37:22 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.1.1 build=1
# Thu, 21 Jan 2021 10:38:56 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Thu, 21 Jan 2021 10:38:56 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Thu, 21 Jan 2021 10:38:56 GMT
WORKDIR /opt/silverpeas/bin
# Thu, 21 Jan 2021 10:38:56 GMT
COPY file:bd0a4d5e9017df7c7d4b9ba1011c737b2e2fcbe0966662e3315fabb5498b8aa3 in /opt/ 
# Thu, 21 Jan 2021 10:38:57 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Thu, 21 Jan 2021 10:41:02 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas construct   && rm ../log/build-*   && touch .install
# Thu, 21 Jan 2021 10:41:02 GMT
EXPOSE 8000 9990
# Thu, 21 Jan 2021 10:41:03 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Thu, 21 Jan 2021 10:41:03 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453ffa30280ef058ed197c390928409b9c7b71a5ab28429d75b2307a47f291b2`  
		Last Modified: Thu, 21 Jan 2021 10:50:17 GMT  
		Size: 482.2 MB (482188669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef987cc50d56d036e369823e849cfb4cb41adf67656e68bc54e53bd7a803e91`  
		Last Modified: Thu, 21 Jan 2021 10:48:55 GMT  
		Size: 4.0 MB (3994026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81079500a3c91140f06b7fbfcc1664569e984a40ecd4e1f6a1983060dfa9a694`  
		Last Modified: Thu, 21 Jan 2021 10:48:54 GMT  
		Size: 7.1 MB (7146628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe187cdb5e1a91b85d3c5bfd66580416a489563d1097ea796dcd082d9189338`  
		Last Modified: Thu, 21 Jan 2021 10:48:51 GMT  
		Size: 490.7 KB (490686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f5f5835de95fd95d76c71aa24e82cd51f100786ff1565a271f93290bc4896c`  
		Last Modified: Thu, 21 Jan 2021 10:48:50 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6169ff8b6b1aaed1447ec19cbcadfe4784a64261c0a8fd4bcb2a1f251d17120`  
		Last Modified: Thu, 21 Jan 2021 10:48:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8066b4330a1965273f00ef9e2246af7c3dd96b7aa28175fa0355791292281518`  
		Last Modified: Thu, 21 Jan 2021 10:49:09 GMT  
		Size: 190.5 MB (190469093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea062f3d89f89c824c360489241820725f7dd8f60c1834d42ed9306b48350d9`  
		Last Modified: Thu, 21 Jan 2021 10:48:49 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d2ca84793979f4ae2a5ab68e164a971879a9ee960ac5797cf31744f46c75ce`  
		Last Modified: Thu, 21 Jan 2021 10:48:49 GMT  
		Size: 759.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a39df8a7f54f3086dbb92c7a3352a3099b1fe88c7af5c4548211b7c8f1ff83`  
		Last Modified: Thu, 21 Jan 2021 10:48:49 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0324f4ddb35888a5fbc04a06467ecc6066fc4092cc1b31ae0273c4c915e28129`  
		Last Modified: Thu, 21 Jan 2021 10:49:45 GMT  
		Size: 716.3 MB (716261302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
