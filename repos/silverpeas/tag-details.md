<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `silverpeas`

-	[`silverpeas:6.0.2`](#silverpeas602)
-	[`silverpeas:6.1.3`](#silverpeas613)
-	[`silverpeas:6.2`](#silverpeas62)
-	[`silverpeas:latest`](#silverpeaslatest)

## `silverpeas:6.0.2`

```console
$ docker pull silverpeas@sha256:eaf61963b49b94b20181fe375d9c7902d307a49a8e7c654453eea1ff8ae5993f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.0.2` - linux; amd64

```console
$ docker pull silverpeas@sha256:b238ef615440d8a981d7564ca0b5c91c76dd37c11ad2c5458c4c9db672d18fb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1014621706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ced3675dc9aadb328642e632034b2f15ac1319b2a5a5563d14e771f63e54482`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:22:16 GMT
ADD file:34f9c325bb2e6ad9f9a062ce9a0237fab0c04aea83f31b8548ea0ae532255be0 in / 
# Fri, 23 Apr 2021 22:22:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:22:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:22:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:22:19 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:39:17 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Sat, 24 Apr 2021 02:39:17 GMT
ENV TERM=xterm
# Sat, 24 Apr 2021 02:42:49 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Sat, 24 Apr 2021 02:42:53 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Sat, 24 Apr 2021 02:42:57 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Sat, 24 Apr 2021 02:42:57 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Sat, 24 Apr 2021 02:43:00 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Sat, 24 Apr 2021 02:43:00 GMT
ENV LANG=en_US.UTF-8
# Sat, 24 Apr 2021 02:43:00 GMT
ENV LANGUAGE=en_US.UTF-8
# Sat, 24 Apr 2021 02:43:00 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 24 Apr 2021 02:43:01 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 24 Apr 2021 02:43:02 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 24 Apr 2021 02:43:02 GMT
ENV JAVA_HOME=/docker-java-home
# Sat, 24 Apr 2021 02:43:02 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Sat, 24 Apr 2021 02:43:03 GMT
ENV JBOSS_HOME=/opt/wildfly
# Sat, 24 Apr 2021 02:43:03 GMT
ENV SILVERPEAS_VERSION=6.0.2
# Sat, 24 Apr 2021 02:43:03 GMT
ENV WILDFLY_VERSION=10.1.0
# Sat, 24 Apr 2021 02:43:03 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.0.2 build=1
# Sat, 24 Apr 2021 02:43:12 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Sat, 24 Apr 2021 02:43:13 GMT
COPY file:d12fb4c8fc28235c5621533a9ae0d98ba26e3adf1ffc690da4a6118aa71d8190 in /root/.m2/ 
# Sat, 24 Apr 2021 02:43:13 GMT
WORKDIR /opt/silverpeas/bin
# Sat, 24 Apr 2021 02:43:13 GMT
COPY file:31e3db287bacfa9fb086f2ae49169410b9f0fdf4178bf47d0ebe93621aa996e4 in /opt/ 
# Sat, 24 Apr 2021 02:43:13 GMT
COPY file:5d883339e9add47c37406a038c7747cafede9f81436843206bab5bde7da6e2f6 in /opt/silverpeas/configuration/silverpeas/ 
# Sat, 24 Apr 2021 02:49:05 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas assemble   && rm ../log/build-*   && touch .install
# Sat, 24 Apr 2021 02:49:08 GMT
EXPOSE 8000 9990
# Sat, 24 Apr 2021 02:49:08 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/xmlcomponents/workflows]
# Sat, 24 Apr 2021 02:49:08 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:92473f7ef45574f608989888a6cfc8187d3a1425e3a63f974434acab03fed068`  
		Last Modified: Sat, 17 Apr 2021 15:20:07 GMT  
		Size: 46.3 MB (46254451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb52bde70123ac7f3a1b88fee95e74f4bdcdbd81917a91a35b56a52ec7671947`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64788f86be3fd71809b5de602deff9445f3de18d2f44a49d0a053dfc9a2008ae`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f6d5f2e001ababe3ddac4731d9c33121e1148ef32a87a83a5b470cb401abef`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6e4ec0d879f58c3ef70fb1c61d6016aece5ffc0dadab4b39efeeb11fbcaad0`  
		Last Modified: Sat, 24 Apr 2021 02:53:27 GMT  
		Size: 207.4 MB (207396446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9f84ef1eaefdbe4d330475b6605461c3ac573e15107393b5ee582b4825a66`  
		Last Modified: Sat, 24 Apr 2021 02:52:58 GMT  
		Size: 4.0 MB (3994083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718db55c345c8f10417bbbd93b286afcf8ebd59c874871780af4784111901fb2`  
		Last Modified: Sat, 24 Apr 2021 02:52:58 GMT  
		Size: 7.1 MB (7146639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b1f9745b0603b73bffe81a139efab5d296180aeb04e6024f959c3991c0f0d9`  
		Last Modified: Sat, 24 Apr 2021 02:52:54 GMT  
		Size: 845.4 KB (845410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ddb8af438157599c7c7e06344ae24e9fc5ed27c1e6d921ce45b9b72b07e925`  
		Last Modified: Sat, 24 Apr 2021 02:52:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9484e606be48d69f3af61e2cf8466e021c8df4f0fd06b2d5d1a7334b9b4b88e6`  
		Last Modified: Sat, 24 Apr 2021 02:52:54 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b21584e100e625e14737525afe9da9682103203a14d2132862988e47b5f6ab`  
		Last Modified: Sat, 24 Apr 2021 02:53:01 GMT  
		Size: 144.3 MB (144284720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a902d0548ee7acb26d5d3b0f47d3f459c18e3d09d720691a056ba1e9707e3ede`  
		Last Modified: Sat, 24 Apr 2021 02:52:51 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cebd52ffc81578a6216b843d8202fb43bbab13595a8b9bff90c4568bda8d17`  
		Last Modified: Sat, 24 Apr 2021 02:52:51 GMT  
		Size: 805.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ab1456674b766338e37b1dd5bbfb63596f68c75e948ee104c88f0c0a50dea2`  
		Last Modified: Sat, 24 Apr 2021 02:52:51 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22d0b8742f1e9f5edded625a240f20f9e76e6d3861cf2d94c87ba9a72a10273`  
		Last Modified: Sat, 24 Apr 2021 02:53:27 GMT  
		Size: 604.7 MB (604696449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:6.1.3`

```console
$ docker pull silverpeas@sha256:e7aef6ef3129f537ff831b903b95a73b147c2678fc945d240f08a6d9b40ce382
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.1.3` - linux; amd64

```console
$ docker pull silverpeas@sha256:84cda2637d42abe415d1e3f988a373b3d769a490c33ff43d1a638ab3df318a04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1426659827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ea294c0750de4ecb85c5837cae19d6ad98b3a497679eacbc2351266c53c9ad9`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:30:03 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Sat, 24 Apr 2021 02:30:04 GMT
ENV TERM=xterm
# Sat, 24 Apr 2021 02:36:40 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Sat, 24 Apr 2021 02:36:48 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Sat, 24 Apr 2021 02:36:52 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Sat, 24 Apr 2021 02:36:52 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Sat, 24 Apr 2021 02:36:55 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Sat, 24 Apr 2021 02:36:55 GMT
ENV LANG=en_US.UTF-8
# Sat, 24 Apr 2021 02:36:55 GMT
ENV LANGUAGE=en_US.UTF-8
# Sat, 24 Apr 2021 02:36:55 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 24 Apr 2021 02:36:56 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 24 Apr 2021 02:36:57 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 24 Apr 2021 02:36:57 GMT
ENV JAVA_HOME=/docker-java-home
# Sat, 24 Apr 2021 02:36:58 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Sat, 24 Apr 2021 02:36:58 GMT
ENV JBOSS_HOME=/opt/wildfly
# Thu, 29 Apr 2021 20:26:06 GMT
ENV SILVERPEAS_VERSION=6.1.3
# Thu, 29 Apr 2021 20:26:06 GMT
ENV WILDFLY_VERSION=18.0.1
# Thu, 29 Apr 2021 20:26:06 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.1.3 build=1
# Thu, 29 Apr 2021 20:26:37 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Thu, 29 Apr 2021 20:26:38 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Thu, 29 Apr 2021 20:26:38 GMT
WORKDIR /opt/silverpeas/bin
# Thu, 29 Apr 2021 20:26:39 GMT
COPY file:bd0a4d5e9017df7c7d4b9ba1011c737b2e2fcbe0966662e3315fabb5498b8aa3 in /opt/ 
# Thu, 29 Apr 2021 20:26:39 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Thu, 29 Apr 2021 20:28:55 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas construct   && rm ../log/build-*   && touch .install
# Thu, 29 Apr 2021 20:28:58 GMT
EXPOSE 8000 9990
# Thu, 29 Apr 2021 20:28:58 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Thu, 29 Apr 2021 20:28:58 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49fc3cb74d31a9bf16c8d7596dc1e945abeb60177726d91c69cdbe8c331e378`  
		Last Modified: Sat, 24 Apr 2021 02:52:42 GMT  
		Size: 481.6 MB (481572759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1ec855de4cf3f900995ae217306b4571fdaec71867d6e0e1f4cbb276b6d2b5`  
		Last Modified: Sat, 24 Apr 2021 02:51:35 GMT  
		Size: 4.0 MB (3994073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277cca691049841c26d247c9c6c3534c8ecabcc34344a70c4f265e90ee56884d`  
		Last Modified: Sat, 24 Apr 2021 02:51:35 GMT  
		Size: 7.1 MB (7146641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfb9850a2084e1c24ed1cb491523344c0ff278485f0f72c8c3559efb20360dd`  
		Last Modified: Sat, 24 Apr 2021 02:51:31 GMT  
		Size: 490.7 KB (490690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2faf5ea23902ba1b8aa1e5a6e36afd4d408d2d9bc275e0dd46d4a304f18610`  
		Last Modified: Sat, 24 Apr 2021 02:51:31 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f16dfab560dbbe82121cb5eb5367b0c3df91d6b887edc3983f4036b431cc23`  
		Last Modified: Sat, 24 Apr 2021 02:51:32 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e705e09ff8f37b4bc69406180c0c9363b01f10395089161e43455604c7867914`  
		Last Modified: Thu, 29 Apr 2021 20:29:27 GMT  
		Size: 190.5 MB (190469424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d9127ab3ac6bd3031d5310a6e21875db3240b0fe85e69f401985d6f3807464`  
		Last Modified: Thu, 29 Apr 2021 20:29:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85a4d2f10f261d4bb8cf0ef754ccad50e22260a0bdcb923d8f68db041cfa88`  
		Last Modified: Thu, 29 Apr 2021 20:29:14 GMT  
		Size: 759.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c943e51d2a332f475fa77bfa4c96534c7fd60d60c5bc4740fa8a3c7d2eb36775`  
		Last Modified: Thu, 29 Apr 2021 20:29:13 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83c16657abe0295b3fb7c1a57b15bd45dfc6c2a884f28436117df21c0578ea1`  
		Last Modified: Thu, 29 Apr 2021 20:29:50 GMT  
		Size: 716.3 MB (716286273 bytes)  
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
