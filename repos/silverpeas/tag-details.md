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
$ docker pull silverpeas@sha256:f642444d4b09436f0940a77a125f34a72bd9ef3d744838d6f5c873d8c60550c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:6.1.3` - linux; amd64

```console
$ docker pull silverpeas@sha256:c40bfa2be23d9f2f63798f38b55ed52df95d3f0aaae5742ec488f4e2a60847bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1426564775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33be8b8feeedaba6cdd91200c965717209b7d11a5e03975f7313a93569f491e9`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:25 GMT
ADD file:dee0aa8497bd26ca41dffa17adff99be2523f66f9b2c557ba9ad2388ed052dca in / 
# Thu, 03 Mar 2022 20:19:25 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 23:43:27 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Thu, 03 Mar 2022 23:43:27 GMT
ENV TERM=xterm
# Thu, 03 Mar 2022 23:50:31 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Thu, 03 Mar 2022 23:50:38 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Thu, 03 Mar 2022 23:50:42 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Thu, 03 Mar 2022 23:50:42 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Thu, 03 Mar 2022 23:50:44 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Thu, 03 Mar 2022 23:50:45 GMT
ENV LANG=en_US.UTF-8
# Thu, 03 Mar 2022 23:50:45 GMT
ENV LANGUAGE=en_US.UTF-8
# Thu, 03 Mar 2022 23:50:45 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 23:50:45 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 03 Mar 2022 23:50:46 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 03 Mar 2022 23:50:46 GMT
ENV JAVA_HOME=/docker-java-home
# Thu, 03 Mar 2022 23:50:46 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Thu, 03 Mar 2022 23:50:46 GMT
ENV JBOSS_HOME=/opt/wildfly
# Thu, 03 Mar 2022 23:50:46 GMT
ENV SILVERPEAS_VERSION=6.1.3
# Thu, 03 Mar 2022 23:50:46 GMT
ENV WILDFLY_VERSION=18.0.1
# Thu, 03 Mar 2022 23:50:46 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.1.3 build=1
# Thu, 03 Mar 2022 23:52:09 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Thu, 03 Mar 2022 23:52:10 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Thu, 03 Mar 2022 23:52:10 GMT
WORKDIR /opt/silverpeas/bin
# Thu, 03 Mar 2022 23:52:10 GMT
COPY file:bd0a4d5e9017df7c7d4b9ba1011c737b2e2fcbe0966662e3315fabb5498b8aa3 in /opt/ 
# Thu, 03 Mar 2022 23:52:10 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Thu, 03 Mar 2022 23:54:27 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas construct   && rm ../log/build-*   && touch .install
# Thu, 03 Mar 2022 23:54:30 GMT
EXPOSE 8000 9990
# Thu, 03 Mar 2022 23:54:30 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Thu, 03 Mar 2022 23:54:30 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:cf06a7c3161117888114e7e91dbd21915efae33c2dbfb086380f7b21946d6e59`  
		Last Modified: Thu, 03 Mar 2022 20:20:28 GMT  
		Size: 26.7 MB (26708326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdbe0d389d8ffcc57fac746c84f75cd1f9344736f09d91bb1e2954ebab0f60b`  
		Last Modified: Thu, 03 Mar 2022 23:57:42 GMT  
		Size: 481.5 MB (481469288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049bdba9e8c15754e29a9ae13acb0e1af50b91c523565fe58ec162b11322fd48`  
		Last Modified: Thu, 03 Mar 2022 23:56:39 GMT  
		Size: 4.0 MB (3994083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a361ea936ece0883755afcd83cdb348071c401d4b5339a76e6af01a6cbb77e5a`  
		Last Modified: Thu, 03 Mar 2022 23:56:40 GMT  
		Size: 7.1 MB (7146665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bf348c0347c8f3d88effa702b8d38c0d948aef9307e25ad5cae55325f5e25`  
		Last Modified: Thu, 03 Mar 2022 23:56:37 GMT  
		Size: 490.7 KB (490693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4405186628dbc28533a7fce51cfcabf456e7f6215a7bd8d0b6fb124255b9fe64`  
		Last Modified: Thu, 03 Mar 2022 23:56:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bce8f41bd2d73305a11ba2c17d46296912709f86e0a07be4acac1466609cde`  
		Last Modified: Thu, 03 Mar 2022 23:56:36 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e486fec1e7fe1a4be37b1c53b3e2e0a9649521a7c1e4244f43ba962c2b0531a`  
		Last Modified: Thu, 03 Mar 2022 23:56:46 GMT  
		Size: 190.5 MB (190469446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96ee710014a04298bd9afd4451a6b4fd649a1b6878707bb9ea8aa44f9c60d56`  
		Last Modified: Thu, 03 Mar 2022 23:56:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78d05fd6589057985c37ec13810876da914748d497f303dea84db6e71c617d2`  
		Last Modified: Thu, 03 Mar 2022 23:56:34 GMT  
		Size: 762.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f600b89e42cc9b350d30f2fca514de5a4b15920699fbe05a30ceee212f78f7c4`  
		Last Modified: Thu, 03 Mar 2022 23:56:34 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a471cc88e47b5d75f373f52290327598bf005ed3b537c2c67a14b22f495beb5`  
		Last Modified: Thu, 03 Mar 2022 23:57:14 GMT  
		Size: 716.3 MB (716284354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:6.2.2`

```console
$ docker pull silverpeas@sha256:7dbe407284e386f0b197001b22382253f10c6ca85711582d4ac941032a9b4bfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `silverpeas:6.2.2` - linux; amd64

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
