<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `silverpeas`

-	[`silverpeas:6.0.2`](#silverpeas602)
-	[`silverpeas:6.1.3`](#silverpeas613)
-	[`silverpeas:6.2.2`](#silverpeas622)
-	[`silverpeas:latest`](#silverpeaslatest)

## `silverpeas:6.0.2`

```console
$ docker pull silverpeas@sha256:b5c9b1df7911d96406247d7fafc0fedda2244be799e6009cfc621ad7be63b0d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:6.0.2` - linux; amd64

```console
$ docker pull silverpeas@sha256:0a267954f687c0500c46dfdb31408a6ce073f519d6d94b7d46feb8f752bd7cb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1014925313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d7219f80b96ae15c804beee33c3e2580723de1295e7a534c385361754e37073`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:03:39 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Tue, 31 Aug 2021 02:03:39 GMT
ENV TERM=xterm
# Tue, 31 Aug 2021 02:07:33 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Tue, 31 Aug 2021 02:07:39 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Tue, 31 Aug 2021 02:07:45 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Tue, 31 Aug 2021 02:07:45 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Tue, 31 Aug 2021 02:07:48 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Tue, 31 Aug 2021 02:07:48 GMT
ENV LANG=en_US.UTF-8
# Tue, 31 Aug 2021 02:07:48 GMT
ENV LANGUAGE=en_US.UTF-8
# Tue, 31 Aug 2021 02:07:48 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 02:07:49 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 31 Aug 2021 02:07:50 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 31 Aug 2021 02:07:50 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 31 Aug 2021 02:07:50 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Tue, 31 Aug 2021 02:07:51 GMT
ENV JBOSS_HOME=/opt/wildfly
# Tue, 31 Aug 2021 02:07:51 GMT
ENV SILVERPEAS_VERSION=6.0.2
# Tue, 31 Aug 2021 02:07:51 GMT
ENV WILDFLY_VERSION=10.1.0
# Tue, 31 Aug 2021 02:07:51 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.0.2 build=1
# Tue, 31 Aug 2021 02:08:09 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Tue, 31 Aug 2021 02:08:10 GMT
COPY file:d12fb4c8fc28235c5621533a9ae0d98ba26e3adf1ffc690da4a6118aa71d8190 in /root/.m2/ 
# Tue, 31 Aug 2021 02:08:10 GMT
WORKDIR /opt/silverpeas/bin
# Tue, 31 Aug 2021 02:08:10 GMT
COPY file:31e3db287bacfa9fb086f2ae49169410b9f0fdf4178bf47d0ebe93621aa996e4 in /opt/ 
# Tue, 31 Aug 2021 02:08:10 GMT
COPY file:5d883339e9add47c37406a038c7747cafede9f81436843206bab5bde7da6e2f6 in /opt/silverpeas/configuration/silverpeas/ 
# Tue, 31 Aug 2021 02:15:29 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas assemble   && rm ../log/build-*   && touch .install
# Tue, 31 Aug 2021 02:15:32 GMT
EXPOSE 8000 9990
# Tue, 31 Aug 2021 02:15:32 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/xmlcomponents/workflows]
# Tue, 31 Aug 2021 02:15:32 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75bab7b2978c6f447f4f11629d5abb18105da46a467b3e7fdad602da38a099a`  
		Last Modified: Tue, 31 Aug 2021 02:19:47 GMT  
		Size: 207.5 MB (207457617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ad3fb77baf164e811362e174b7f55078faddfb5419581e02ee8be4e22c8cb`  
		Last Modified: Tue, 31 Aug 2021 02:19:19 GMT  
		Size: 4.0 MB (3994087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa21a02eb15eabcb08194dc549f6d2633401a9f02b70a28c42acfb982a2c0892`  
		Last Modified: Tue, 31 Aug 2021 02:19:19 GMT  
		Size: 7.1 MB (7146644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957309a7c22133ea5da921a9e1c440e5db36c1ef29767922a96d0715144a7f3c`  
		Last Modified: Tue, 31 Aug 2021 02:19:15 GMT  
		Size: 845.4 KB (845399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f504f19b2261f336d5fb8ed204508a177d4672a306b41a359f41940d39c67f`  
		Last Modified: Tue, 31 Aug 2021 02:19:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07658715bda815de3e29d8e151f013b1b5ef7fc70e9b567fc532bb8bd19e2c04`  
		Last Modified: Tue, 31 Aug 2021 02:19:15 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f600e097c39adc1a81b28bad70ec252868df7c4824d28038502d09de60f0e340`  
		Last Modified: Tue, 31 Aug 2021 02:19:21 GMT  
		Size: 144.3 MB (144284714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa2533c95124d7f6f1f71e873889eb02fb290464f44877ab8db60dc9c58931f`  
		Last Modified: Tue, 31 Aug 2021 02:19:13 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a055b4aee299167cc171b4c496a6fa722dc1cafaffba88430008c4671edfd5d6`  
		Last Modified: Tue, 31 Aug 2021 02:19:12 GMT  
		Size: 809.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f3514ac10d9002bc266d0d7d3916e143b49a339e7cc5249b412b4699987d38`  
		Last Modified: Tue, 31 Aug 2021 02:19:12 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af73964675c4218dd30a52c94723697d58cf2d0cd23cf4a61cb6da0396cf0aa`  
		Last Modified: Tue, 31 Aug 2021 02:19:44 GMT  
		Size: 604.7 MB (604695778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:6.1.3`

```console
$ docker pull silverpeas@sha256:5c00c5dcc0488f49fab9cb135abdbfe5869559754aa25e70456f91bc6d4bf225
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:6.1.3` - linux; amd64

```console
$ docker pull silverpeas@sha256:aafc6f12a87115c85b4841089c20d547607aeab5320387fd5a7066a2feac432b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1426527378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94fd9b83484ffec91ddb6c43842084bdb3088b9e47a9faa9a84bbef28c38c322`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:39:43 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Fri, 01 Oct 2021 06:39:43 GMT
ENV TERM=xterm
# Fri, 01 Oct 2021 06:46:35 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Fri, 01 Oct 2021 06:46:43 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Fri, 01 Oct 2021 06:46:48 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Fri, 01 Oct 2021 06:46:48 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Fri, 01 Oct 2021 06:46:51 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Fri, 01 Oct 2021 06:46:51 GMT
ENV LANG=en_US.UTF-8
# Fri, 01 Oct 2021 06:46:51 GMT
ENV LANGUAGE=en_US.UTF-8
# Fri, 01 Oct 2021 06:46:51 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 01 Oct 2021 06:46:52 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 01 Oct 2021 06:46:53 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 01 Oct 2021 06:46:53 GMT
ENV JAVA_HOME=/docker-java-home
# Fri, 01 Oct 2021 06:46:53 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Fri, 01 Oct 2021 06:46:53 GMT
ENV JBOSS_HOME=/opt/wildfly
# Fri, 01 Oct 2021 06:46:54 GMT
ENV SILVERPEAS_VERSION=6.1.3
# Fri, 01 Oct 2021 06:46:54 GMT
ENV WILDFLY_VERSION=18.0.1
# Fri, 01 Oct 2021 06:46:54 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.1.3 build=1
# Fri, 01 Oct 2021 06:47:06 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Fri, 01 Oct 2021 06:47:06 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Fri, 01 Oct 2021 06:47:07 GMT
WORKDIR /opt/silverpeas/bin
# Fri, 01 Oct 2021 06:47:07 GMT
COPY file:bd0a4d5e9017df7c7d4b9ba1011c737b2e2fcbe0966662e3315fabb5498b8aa3 in /opt/ 
# Fri, 01 Oct 2021 06:47:07 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Fri, 01 Oct 2021 06:49:12 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas construct   && rm ../log/build-*   && touch .install
# Fri, 01 Oct 2021 06:49:15 GMT
EXPOSE 8000 9990
# Fri, 01 Oct 2021 06:49:15 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Fri, 01 Oct 2021 06:49:16 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce7ee3ef1a33565f839bcf009b3c75d659e9d924e52681bdd1a22da22fdc14a`  
		Last Modified: Fri, 01 Oct 2021 06:52:38 GMT  
		Size: 481.4 MB (481434072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59a7786b48cde3d9ca14992177d08b30380c1d94e3694a1b0762dd835c38613`  
		Last Modified: Fri, 01 Oct 2021 06:51:35 GMT  
		Size: 4.0 MB (3994087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5167bb41abe70ae0b9d3fcbc9d7c75f59b6b2caf59aadf6ee21696c9f496550`  
		Last Modified: Fri, 01 Oct 2021 06:51:35 GMT  
		Size: 7.1 MB (7146659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce84ec10b80deb7767df032ac556c88216eaf15543185e9a5afff3ad6d2b693`  
		Last Modified: Fri, 01 Oct 2021 06:51:32 GMT  
		Size: 490.7 KB (490685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f513859d07e6989fe48216e07bb460687b7c360dc809fb2d7ca8898a2a9cb25`  
		Last Modified: Fri, 01 Oct 2021 06:51:31 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecbc9d2ad5d663f2af43733e9b0e0bbca75d45eb3f8601fab02b888663e4cae`  
		Last Modified: Fri, 01 Oct 2021 06:51:31 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6d7beadfe3050a9fb4958f0b53e9ebe6e52b9ac9f0bc5e6b8b7b61785e0f76`  
		Last Modified: Fri, 01 Oct 2021 06:51:42 GMT  
		Size: 190.5 MB (190469435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026d202040a0768bc993914864b06b1b19980098131db9fd1275b4a9816b2bf2`  
		Last Modified: Fri, 01 Oct 2021 06:51:29 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d252facd361dbc316ffee6430f3327c47f64438bf2b621eab143bab570717635`  
		Last Modified: Fri, 01 Oct 2021 06:51:29 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84e3914595700845c370bbac8e4a3175f8b6645c4d5160fef543d77fe20c303`  
		Last Modified: Fri, 01 Oct 2021 06:51:29 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b150e11337453b8d7a306b9d0332b7e5985fc1ffab7a15b8cf2088db748ca88a`  
		Last Modified: Fri, 01 Oct 2021 06:52:06 GMT  
		Size: 716.3 MB (716285444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:6.2.2`

```console
$ docker pull silverpeas@sha256:1ffd3e94c87c3797051c0b0964c2551f2cc803a20af27e52c8e9c1210d5d5fd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:6.2.2` - linux; amd64

```console
$ docker pull silverpeas@sha256:315ba837d2e545213ea1b8b52acdb7fa989ed3f20fb36edf29ad8fdbebb4366d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1896844292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e87c410141b6a98f5aa79be4f7fbe890295eec65255b96171c140c7d67a83bc1`
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
# Fri, 17 Dec 2021 23:19:55 GMT
ENV SILVERPEAS_VERSION=6.2.2
# Fri, 17 Dec 2021 23:19:55 GMT
ENV WILDFLY_VERSION=20.0.1
# Fri, 17 Dec 2021 23:19:55 GMT
LABEL name=Silverpeas 6.2.2 description=Image to install and to run Silverpeas 6.2.2 vendor=Silverpeas version=6.2.2 build=1
# Fri, 17 Dec 2021 23:20:10 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Fri, 17 Dec 2021 23:20:11 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Fri, 17 Dec 2021 23:20:11 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Fri, 17 Dec 2021 23:20:12 GMT
WORKDIR /opt/silverpeas/bin
# Fri, 17 Dec 2021 23:20:12 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Fri, 17 Dec 2021 23:20:12 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Fri, 17 Dec 2021 23:22:03 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Fri, 17 Dec 2021 23:22:06 GMT
EXPOSE 8000 9990
# Fri, 17 Dec 2021 23:22:07 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Fri, 17 Dec 2021 23:22:07 GMT
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
	-	`sha256:3bf7c10b4d8f1db1bf6ded9d75806109c1732d1eabbc7998ade095a54276f60c`  
		Last Modified: Fri, 17 Dec 2021 23:22:42 GMT  
		Size: 196.8 MB (196774062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cf9982bcf67a3896b9e9c80776f2c074ad135f58057d0374c02f4b59569865`  
		Last Modified: Fri, 17 Dec 2021 23:22:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dd446b29fd7915c2d8b848962ec10c7a31cbd38720bc4b95fd9ecf7b52fc52`  
		Last Modified: Fri, 17 Dec 2021 23:22:29 GMT  
		Size: 660.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca1b217b4ebe92bacc674d9177aee670e97eb1efa6059fa3872404cf38100e0`  
		Last Modified: Fri, 17 Dec 2021 23:22:29 GMT  
		Size: 875.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83dcc7964c7e4c98bbc54f505711a78b244f7e8667eec6bea0243891388adfe8`  
		Last Modified: Fri, 17 Dec 2021 23:22:29 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ce9bbf5659c57125a395ea40a7f95dc31b18ca64a0b94083bb59ca3bef6ee`  
		Last Modified: Fri, 17 Dec 2021 23:23:03 GMT  
		Size: 748.0 MB (748022440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:1ffd3e94c87c3797051c0b0964c2551f2cc803a20af27e52c8e9c1210d5d5fd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:315ba837d2e545213ea1b8b52acdb7fa989ed3f20fb36edf29ad8fdbebb4366d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1896844292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e87c410141b6a98f5aa79be4f7fbe890295eec65255b96171c140c7d67a83bc1`
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
# Fri, 17 Dec 2021 23:19:55 GMT
ENV SILVERPEAS_VERSION=6.2.2
# Fri, 17 Dec 2021 23:19:55 GMT
ENV WILDFLY_VERSION=20.0.1
# Fri, 17 Dec 2021 23:19:55 GMT
LABEL name=Silverpeas 6.2.2 description=Image to install and to run Silverpeas 6.2.2 vendor=Silverpeas version=6.2.2 build=1
# Fri, 17 Dec 2021 23:20:10 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Fri, 17 Dec 2021 23:20:11 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Fri, 17 Dec 2021 23:20:11 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Fri, 17 Dec 2021 23:20:12 GMT
WORKDIR /opt/silverpeas/bin
# Fri, 17 Dec 2021 23:20:12 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Fri, 17 Dec 2021 23:20:12 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Fri, 17 Dec 2021 23:22:03 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Fri, 17 Dec 2021 23:22:06 GMT
EXPOSE 8000 9990
# Fri, 17 Dec 2021 23:22:07 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Fri, 17 Dec 2021 23:22:07 GMT
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
	-	`sha256:3bf7c10b4d8f1db1bf6ded9d75806109c1732d1eabbc7998ade095a54276f60c`  
		Last Modified: Fri, 17 Dec 2021 23:22:42 GMT  
		Size: 196.8 MB (196774062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cf9982bcf67a3896b9e9c80776f2c074ad135f58057d0374c02f4b59569865`  
		Last Modified: Fri, 17 Dec 2021 23:22:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dd446b29fd7915c2d8b848962ec10c7a31cbd38720bc4b95fd9ecf7b52fc52`  
		Last Modified: Fri, 17 Dec 2021 23:22:29 GMT  
		Size: 660.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca1b217b4ebe92bacc674d9177aee670e97eb1efa6059fa3872404cf38100e0`  
		Last Modified: Fri, 17 Dec 2021 23:22:29 GMT  
		Size: 875.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83dcc7964c7e4c98bbc54f505711a78b244f7e8667eec6bea0243891388adfe8`  
		Last Modified: Fri, 17 Dec 2021 23:22:29 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ce9bbf5659c57125a395ea40a7f95dc31b18ca64a0b94083bb59ca3bef6ee`  
		Last Modified: Fri, 17 Dec 2021 23:23:03 GMT  
		Size: 748.0 MB (748022440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
