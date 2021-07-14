<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `silverpeas`

-	[`silverpeas:6.0.2`](#silverpeas602)
-	[`silverpeas:6.1.3`](#silverpeas613)
-	[`silverpeas:6.2.1`](#silverpeas621)
-	[`silverpeas:latest`](#silverpeaslatest)

## `silverpeas:6.0.2`

```console
$ docker pull silverpeas@sha256:f969484de3c9739d5145664ee2265f3c00cdf6b72e5072378ada903ef31e5f13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.0.2` - linux; amd64

```console
$ docker pull silverpeas@sha256:5ef70de7fc5a8fda4e5d262f376ff12910393ce2781d18e4d9242af56aae3290
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1014923558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0fe5773c74c481da9d067b2704504c16970645e4811b68998709a398c7e990`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 02:55:45 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Fri, 18 Jun 2021 02:55:45 GMT
ENV TERM=xterm
# Fri, 18 Jun 2021 02:59:23 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Fri, 18 Jun 2021 02:59:28 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Fri, 18 Jun 2021 02:59:32 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Fri, 18 Jun 2021 02:59:32 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Fri, 18 Jun 2021 02:59:35 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Fri, 18 Jun 2021 02:59:35 GMT
ENV LANG=en_US.UTF-8
# Fri, 18 Jun 2021 02:59:35 GMT
ENV LANGUAGE=en_US.UTF-8
# Fri, 18 Jun 2021 02:59:36 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 18 Jun 2021 02:59:37 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 18 Jun 2021 02:59:38 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 18 Jun 2021 02:59:38 GMT
ENV JAVA_HOME=/docker-java-home
# Fri, 18 Jun 2021 02:59:38 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Fri, 18 Jun 2021 02:59:38 GMT
ENV JBOSS_HOME=/opt/wildfly
# Fri, 18 Jun 2021 02:59:38 GMT
ENV SILVERPEAS_VERSION=6.0.2
# Fri, 18 Jun 2021 02:59:38 GMT
ENV WILDFLY_VERSION=10.1.0
# Fri, 18 Jun 2021 02:59:39 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.0.2 build=1
# Fri, 18 Jun 2021 02:59:58 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Fri, 18 Jun 2021 02:59:58 GMT
COPY file:d12fb4c8fc28235c5621533a9ae0d98ba26e3adf1ffc690da4a6118aa71d8190 in /root/.m2/ 
# Fri, 18 Jun 2021 02:59:59 GMT
WORKDIR /opt/silverpeas/bin
# Fri, 18 Jun 2021 02:59:59 GMT
COPY file:31e3db287bacfa9fb086f2ae49169410b9f0fdf4178bf47d0ebe93621aa996e4 in /opt/ 
# Fri, 18 Jun 2021 02:59:59 GMT
COPY file:5d883339e9add47c37406a038c7747cafede9f81436843206bab5bde7da6e2f6 in /opt/silverpeas/configuration/silverpeas/ 
# Fri, 18 Jun 2021 03:06:10 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas assemble   && rm ../log/build-*   && touch .install
# Fri, 18 Jun 2021 03:06:12 GMT
EXPOSE 8000 9990
# Fri, 18 Jun 2021 03:06:13 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/xmlcomponents/workflows]
# Fri, 18 Jun 2021 03:06:13 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d118cc87cf52b53fd1b3cc141ba7bc9121397b185294b0db53a34fe042cea46`  
		Last Modified: Fri, 18 Jun 2021 03:10:31 GMT  
		Size: 207.5 MB (207456151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd04fe4e7236586c978be3fde6fd719b689cf08b556f2e8511a0cfa79cad0656`  
		Last Modified: Fri, 18 Jun 2021 03:10:01 GMT  
		Size: 4.0 MB (3994089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61518036d758e4c58f3f64a744a7e103ed43dd58b352b98d22120ba59214d56`  
		Last Modified: Fri, 18 Jun 2021 03:10:02 GMT  
		Size: 7.1 MB (7146655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7c0bc726ebb4d9dfdb54ae20a7cee96ef7954c1a23b58263fbdebb4b9f9380`  
		Last Modified: Fri, 18 Jun 2021 03:09:58 GMT  
		Size: 845.4 KB (845434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dacea640ec8e66d314408263d553fd43643718425452f6273767e4d11c214ab2`  
		Last Modified: Fri, 18 Jun 2021 03:09:57 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81a4402d3b510f1d06e07480bb916c6b9155135326ceba80a2809eaf05258b9`  
		Last Modified: Fri, 18 Jun 2021 03:09:57 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7444b2257cc2c7f47eacca62722621663ce633ef2b2660eb86446ecfc22164`  
		Last Modified: Fri, 18 Jun 2021 03:10:05 GMT  
		Size: 144.3 MB (144284706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e82ed5277996b2db7fcb8a0a3e28b61224969b0b06c10b9499d018c2f017f3`  
		Last Modified: Fri, 18 Jun 2021 03:09:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4a42f00372f9d9efa4aca5b32df4821dec543ea52f2080d82a992def118833`  
		Last Modified: Fri, 18 Jun 2021 03:09:55 GMT  
		Size: 808.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab6810f19321b9c4ae821e603e830a58a5e7a255498b231b26e7a433d42e408`  
		Last Modified: Fri, 18 Jun 2021 03:09:55 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c3adf0b3119b138f9a1b5e2a9948e70da9fac4977ef0219c7da2093338889e`  
		Last Modified: Fri, 18 Jun 2021 03:10:28 GMT  
		Size: 604.7 MB (604696226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:6.1.3`

```console
$ docker pull silverpeas@sha256:138bfc98343cd8d0efc65ce8a1b851cb923b6c160481a478235d5b1accad076b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.1.3` - linux; amd64

```console
$ docker pull silverpeas@sha256:1ace49045e01115629ef2721bebd4091a5ed4c32ea5d4c4944d4c11511251234
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1426542505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4214dbf6eea0156beee071480491545fc156aa1b1b3782094564c21a9d9731b6`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:37:40 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Wed, 14 Jul 2021 01:37:40 GMT
ENV TERM=xterm
# Wed, 14 Jul 2021 01:44:39 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Wed, 14 Jul 2021 01:44:48 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Wed, 14 Jul 2021 01:44:53 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Wed, 14 Jul 2021 01:44:54 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Wed, 14 Jul 2021 01:44:59 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Wed, 14 Jul 2021 01:44:59 GMT
ENV LANG=en_US.UTF-8
# Wed, 14 Jul 2021 01:45:00 GMT
ENV LANGUAGE=en_US.UTF-8
# Wed, 14 Jul 2021 01:45:00 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 14 Jul 2021 01:45:01 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 14 Jul 2021 01:45:02 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 14 Jul 2021 01:45:03 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 14 Jul 2021 01:45:03 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Wed, 14 Jul 2021 01:45:03 GMT
ENV JBOSS_HOME=/opt/wildfly
# Wed, 14 Jul 2021 01:45:03 GMT
ENV SILVERPEAS_VERSION=6.1.3
# Wed, 14 Jul 2021 01:45:04 GMT
ENV WILDFLY_VERSION=18.0.1
# Wed, 14 Jul 2021 01:45:04 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.1.3 build=1
# Wed, 14 Jul 2021 01:45:16 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Wed, 14 Jul 2021 01:45:16 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Wed, 14 Jul 2021 01:45:17 GMT
WORKDIR /opt/silverpeas/bin
# Wed, 14 Jul 2021 01:45:17 GMT
COPY file:bd0a4d5e9017df7c7d4b9ba1011c737b2e2fcbe0966662e3315fabb5498b8aa3 in /opt/ 
# Wed, 14 Jul 2021 01:45:17 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Wed, 14 Jul 2021 01:47:35 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas construct   && rm ../log/build-*   && touch .install
# Wed, 14 Jul 2021 01:47:40 GMT
EXPOSE 8000 9990
# Wed, 14 Jul 2021 01:47:40 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Wed, 14 Jul 2021 01:47:41 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98034b29a67aca6d3fd1eff301a37488f530c5d9502fd4d9f32d2018e930f173`  
		Last Modified: Wed, 14 Jul 2021 01:53:05 GMT  
		Size: 481.4 MB (481443420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1ac6a1d3318a8b67d341239831c73458e956ce5e4c33f0d4e4596b7e284774`  
		Last Modified: Wed, 14 Jul 2021 01:51:15 GMT  
		Size: 4.0 MB (3994066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb22d48886b51bfe5c7e977ab88e52d2ff150a062594b343138abff394c21d7`  
		Last Modified: Wed, 14 Jul 2021 01:51:16 GMT  
		Size: 7.1 MB (7146663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2e79bc2864b0179aa0a2ba4975a032a4eb380a4114c12a45efb46ff384e48a`  
		Last Modified: Wed, 14 Jul 2021 01:51:10 GMT  
		Size: 490.7 KB (490688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025d1779015254aaaa2f5f3aa93ddcb39ac467fbee0a5d3cb229e8cd1d054c12`  
		Last Modified: Wed, 14 Jul 2021 01:51:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d5a1a0e197cbc646cc3d896db4d63ec8f470a1ae44e76bdd4b19835c7d52d6`  
		Last Modified: Wed, 14 Jul 2021 01:51:10 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe5e27655fda83756793f7fe7ba3c6f755f151db177039478109d4c8c020c7a`  
		Last Modified: Wed, 14 Jul 2021 01:51:30 GMT  
		Size: 190.5 MB (190469418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea46fe66b04a2e25155d1e9312889843d59aa80658d36b6b4e5f3a9701aa0c9`  
		Last Modified: Wed, 14 Jul 2021 01:51:07 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d0ef13a95881b7673c3d5f9c0d50a3f6acb440a804b289ca2e6dbd89e80fc8`  
		Last Modified: Wed, 14 Jul 2021 01:51:07 GMT  
		Size: 759.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f2d15335a6675320b4f9f87a3d97ddde3552bf95f12fb1622d6437b2a40cd6`  
		Last Modified: Wed, 14 Jul 2021 01:51:07 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351fb7234f3e9d3e05cae6bb9b9bab1c194226c30d5af203f502be3fb577678`  
		Last Modified: Wed, 14 Jul 2021 01:52:20 GMT  
		Size: 716.3 MB (716290186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:6.2.1`

```console
$ docker pull silverpeas@sha256:9477b1b7959d46e0a5d34cffdd0557a5b2a4cce68c1918a97fbc1c5a8d99cc2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.2.1` - linux; amd64

```console
$ docker pull silverpeas@sha256:1ea0dfe2fb20ee53d8ade045bcf0407345a7d7c8c1f6203c036be745b3c9659d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1884481607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f93585539efb8efb5ec199c5bcbef622e1158f9db328a265572da1b6d1776ebe`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:23:40 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Wed, 14 Jul 2021 01:23:40 GMT
ENV TERM=xterm
# Wed, 14 Jul 2021 01:31:49 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Wed, 14 Jul 2021 01:31:55 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Wed, 14 Jul 2021 01:31:59 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Wed, 14 Jul 2021 01:31:59 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Wed, 14 Jul 2021 01:32:37 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Wed, 14 Jul 2021 01:32:37 GMT
ENV LANG=en_US.UTF-8
# Wed, 14 Jul 2021 01:32:38 GMT
ENV LANGUAGE=en_US.UTF-8
# Wed, 14 Jul 2021 01:32:38 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 14 Jul 2021 01:32:39 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 14 Jul 2021 01:32:40 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 14 Jul 2021 01:32:40 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 14 Jul 2021 01:32:40 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Wed, 14 Jul 2021 01:32:40 GMT
ENV JBOSS_HOME=/opt/wildfly
# Wed, 14 Jul 2021 01:32:40 GMT
ENV SILVERPEAS_VERSION=6.2.1
# Wed, 14 Jul 2021 01:32:41 GMT
ENV WILDFLY_VERSION=20.0.1
# Wed, 14 Jul 2021 01:32:41 GMT
LABEL name=Silverpeas 6.2.1 description=Image to install and to run Silverpeas 6.2.1 vendor=Silverpeas version=6.2.1 build=1
# Wed, 14 Jul 2021 01:33:47 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Wed, 14 Jul 2021 01:33:48 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Wed, 14 Jul 2021 01:33:48 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Wed, 14 Jul 2021 01:33:48 GMT
WORKDIR /opt/silverpeas/bin
# Wed, 14 Jul 2021 01:33:48 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Wed, 14 Jul 2021 01:33:49 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Wed, 14 Jul 2021 01:37:24 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Wed, 14 Jul 2021 01:37:27 GMT
EXPOSE 8000 9990
# Wed, 14 Jul 2021 01:37:28 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Wed, 14 Jul 2021 01:37:28 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63315563f686b6df7e360010cf3c4e0d4c7afe6cff14f3427271d1feb5263db`  
		Last Modified: Wed, 14 Jul 2021 01:50:51 GMT  
		Size: 905.0 MB (905002332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5e3f537ae2f00db262cef31d830d5c4410eca2426ca6474157bdb02d763101`  
		Last Modified: Wed, 14 Jul 2021 01:48:10 GMT  
		Size: 4.0 MB (3994078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73be137c4c0dd0070b39d1f8766a62d15e104c6fa71668a645dc23c4497f9bce`  
		Last Modified: Wed, 14 Jul 2021 01:48:12 GMT  
		Size: 7.1 MB (7146640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e208b33bac3665b4fbfd58ed76f3f87af5eca3236f3e051113a1278409bb99bc`  
		Last Modified: Wed, 14 Jul 2021 01:48:07 GMT  
		Size: 2.5 MB (2534362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d748dbb483f710155ce54ad649f377e34ed9c48812904f40f8132d96ab398207`  
		Last Modified: Wed, 14 Jul 2021 01:48:07 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc67649011245a7a96c8e38bc8871ebd3f0e405bac1508763c29a365b504c8bd`  
		Last Modified: Wed, 14 Jul 2021 01:48:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e71ec127e4db7907ab7f16c8d2def43fc9e71564a711a43ad425c0e743a4de`  
		Last Modified: Wed, 14 Jul 2021 01:48:27 GMT  
		Size: 196.8 MB (196774063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355633a622a9ecb83bf5e9e5c5a8b2ebbadf39e59379a09104fb67f4f17ff644`  
		Last Modified: Wed, 14 Jul 2021 01:48:04 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9eea583adb0331d5c6653ba0594fb92d81d3c3333f4f662a2316567ddbc2ba6`  
		Last Modified: Wed, 14 Jul 2021 01:48:04 GMT  
		Size: 662.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a82b9126d6506a9de7aa34a92e85cb859c1f0ca3f9d826bc223dc81766d144`  
		Last Modified: Wed, 14 Jul 2021 01:48:04 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f9e7c1482ef4791d4032a4667ca93e3f695384ac597213c5d1a5bd952043b`  
		Last Modified: Wed, 14 Jul 2021 01:48:04 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c204d0ab60cc3bb47ec05655d0f7779a1b49d6e927b930ea6b0bdde20b3664`  
		Last Modified: Wed, 14 Jul 2021 01:49:16 GMT  
		Size: 740.5 MB (740461568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:9477b1b7959d46e0a5d34cffdd0557a5b2a4cce68c1918a97fbc1c5a8d99cc2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:1ea0dfe2fb20ee53d8ade045bcf0407345a7d7c8c1f6203c036be745b3c9659d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1884481607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f93585539efb8efb5ec199c5bcbef622e1158f9db328a265572da1b6d1776ebe`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:23:40 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Wed, 14 Jul 2021 01:23:40 GMT
ENV TERM=xterm
# Wed, 14 Jul 2021 01:31:49 GMT
RUN apt-get update   && apt-get install -y tzdata   && apt-get install -y     apt-utils     iputils-ping     curl     wget     vim     locales     language-pack-en     language-pack-fr     procps     net-tools     zip     unzip     openjdk-11-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Wed, 14 Jul 2021 01:31:55 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Wed, 14 Jul 2021 01:31:59 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Wed, 14 Jul 2021 01:31:59 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Wed, 14 Jul 2021 01:32:37 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Wed, 14 Jul 2021 01:32:37 GMT
ENV LANG=en_US.UTF-8
# Wed, 14 Jul 2021 01:32:38 GMT
ENV LANGUAGE=en_US.UTF-8
# Wed, 14 Jul 2021 01:32:38 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 14 Jul 2021 01:32:39 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 14 Jul 2021 01:32:40 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 14 Jul 2021 01:32:40 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 14 Jul 2021 01:32:40 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Wed, 14 Jul 2021 01:32:40 GMT
ENV JBOSS_HOME=/opt/wildfly
# Wed, 14 Jul 2021 01:32:40 GMT
ENV SILVERPEAS_VERSION=6.2.1
# Wed, 14 Jul 2021 01:32:41 GMT
ENV WILDFLY_VERSION=20.0.1
# Wed, 14 Jul 2021 01:32:41 GMT
LABEL name=Silverpeas 6.2.1 description=Image to install and to run Silverpeas 6.2.1 vendor=Silverpeas version=6.2.1 build=1
# Wed, 14 Jul 2021 01:33:47 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Wed, 14 Jul 2021 01:33:48 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Wed, 14 Jul 2021 01:33:48 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Wed, 14 Jul 2021 01:33:48 GMT
WORKDIR /opt/silverpeas/bin
# Wed, 14 Jul 2021 01:33:48 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Wed, 14 Jul 2021 01:33:49 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Wed, 14 Jul 2021 01:37:24 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && rm ../log/build-*   && touch .install
# Wed, 14 Jul 2021 01:37:27 GMT
EXPOSE 8000 9990
# Wed, 14 Jul 2021 01:37:28 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Wed, 14 Jul 2021 01:37:28 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63315563f686b6df7e360010cf3c4e0d4c7afe6cff14f3427271d1feb5263db`  
		Last Modified: Wed, 14 Jul 2021 01:50:51 GMT  
		Size: 905.0 MB (905002332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5e3f537ae2f00db262cef31d830d5c4410eca2426ca6474157bdb02d763101`  
		Last Modified: Wed, 14 Jul 2021 01:48:10 GMT  
		Size: 4.0 MB (3994078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73be137c4c0dd0070b39d1f8766a62d15e104c6fa71668a645dc23c4497f9bce`  
		Last Modified: Wed, 14 Jul 2021 01:48:12 GMT  
		Size: 7.1 MB (7146640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e208b33bac3665b4fbfd58ed76f3f87af5eca3236f3e051113a1278409bb99bc`  
		Last Modified: Wed, 14 Jul 2021 01:48:07 GMT  
		Size: 2.5 MB (2534362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d748dbb483f710155ce54ad649f377e34ed9c48812904f40f8132d96ab398207`  
		Last Modified: Wed, 14 Jul 2021 01:48:07 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc67649011245a7a96c8e38bc8871ebd3f0e405bac1508763c29a365b504c8bd`  
		Last Modified: Wed, 14 Jul 2021 01:48:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e71ec127e4db7907ab7f16c8d2def43fc9e71564a711a43ad425c0e743a4de`  
		Last Modified: Wed, 14 Jul 2021 01:48:27 GMT  
		Size: 196.8 MB (196774063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355633a622a9ecb83bf5e9e5c5a8b2ebbadf39e59379a09104fb67f4f17ff644`  
		Last Modified: Wed, 14 Jul 2021 01:48:04 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9eea583adb0331d5c6653ba0594fb92d81d3c3333f4f662a2316567ddbc2ba6`  
		Last Modified: Wed, 14 Jul 2021 01:48:04 GMT  
		Size: 662.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a82b9126d6506a9de7aa34a92e85cb859c1f0ca3f9d826bc223dc81766d144`  
		Last Modified: Wed, 14 Jul 2021 01:48:04 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f9e7c1482ef4791d4032a4667ca93e3f695384ac597213c5d1a5bd952043b`  
		Last Modified: Wed, 14 Jul 2021 01:48:04 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c204d0ab60cc3bb47ec05655d0f7779a1b49d6e927b930ea6b0bdde20b3664`  
		Last Modified: Wed, 14 Jul 2021 01:49:16 GMT  
		Size: 740.5 MB (740461568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
