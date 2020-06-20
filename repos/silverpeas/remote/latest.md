## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:ba87ed6c335178fdc1de213c8c409ea1b772034b942eeaadcf3bb23e88be2efe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:7bc2471bf399e5d3af9f8934e109baa3efb845adf6f1dfad0e3e6eecb1a4a6e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1437785821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394ba39f4e967e0c6cc6d0034cd6b6c4e15bd7f8c3559c2285531d023bb04b50`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Sat, 20 Jun 2020 00:20:02 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Sat, 20 Jun 2020 00:20:03 GMT
ENV TERM=xterm
# Sat, 20 Jun 2020 00:24:34 GMT
RUN apt-get update && apt-get install -y     wget     vim     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Sat, 20 Jun 2020 00:24:41 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Sat, 20 Jun 2020 00:25:08 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Sat, 20 Jun 2020 00:25:09 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Sat, 20 Jun 2020 00:25:12 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Sat, 20 Jun 2020 00:25:12 GMT
ENV LANG=en_US.UTF-8
# Sat, 20 Jun 2020 00:25:12 GMT
ENV LANGUAGE=en_US.UTF-8
# Sat, 20 Jun 2020 00:25:12 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 20 Jun 2020 00:25:13 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 20 Jun 2020 00:25:14 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 20 Jun 2020 00:25:14 GMT
ENV JAVA_HOME=/docker-java-home
# Sat, 20 Jun 2020 00:25:14 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Sat, 20 Jun 2020 00:25:14 GMT
ENV JBOSS_HOME=/opt/wildfly
# Sat, 20 Jun 2020 00:25:14 GMT
ENV SILVERPEAS_VERSION=6.1
# Sat, 20 Jun 2020 00:25:14 GMT
ENV WILDFLY_VERSION=18.0.1
# Sat, 20 Jun 2020 00:25:15 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.1 build=2
# Sat, 20 Jun 2020 00:25:58 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Sat, 20 Jun 2020 00:25:58 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Sat, 20 Jun 2020 00:25:58 GMT
COPY file:473bf75b335a39b6b4b39c64cd151bd8ed3d3e33da73b8124e537a5db1fad3d6 in /opt/silverpeas/bin/ 
# Sat, 20 Jun 2020 00:25:58 GMT
WORKDIR /opt/silverpeas/bin
# Sat, 20 Jun 2020 00:25:59 GMT
COPY file:b54156953ecf6c3259f3b3d2885a784847c0996fd145c0f7ccef25182725511f in /opt/ 
# Sat, 20 Jun 2020 00:25:59 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Sat, 20 Jun 2020 00:36:05 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN sed -i -e "s/SILVERPEAS_VERSION/${SILVERPEAS_VERSION}/g" ${SILVERPEAS_HOME}/bin/silverpeas.gradle   && ./silverpeas construct   && mv ../migrations/db/h2/busCore/up040/alter-table.sql ../migrations/db/h2/busCore/up040/alter_table.sql   && rm ../log/build-*   && touch .install
# Sat, 20 Jun 2020 00:36:06 GMT
EXPOSE 8000 9990
# Sat, 20 Jun 2020 00:36:06 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Sat, 20 Jun 2020 00:36:07 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c7b0cf439de107666ddad6bdc73d1c5bceec0b794d5f71c613fadc91ce7ef7`  
		Last Modified: Sat, 20 Jun 2020 00:37:55 GMT  
		Size: 489.4 MB (489371817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0f16fc5f6a4ca80acd79dde25f20c04cfa45ef9276f936713283b251352b31`  
		Last Modified: Sat, 20 Jun 2020 00:36:29 GMT  
		Size: 4.0 MB (3994026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50950049ddfb6ada7c3593e0d47c213377f2b3f000f051a37d0aee6328c7485`  
		Last Modified: Sat, 20 Jun 2020 00:36:29 GMT  
		Size: 7.1 MB (7146625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2b3c69e4fea3aef7ac698fa26c519d47d718749dd5dcc221d45a1f08c19c52`  
		Last Modified: Sat, 20 Jun 2020 00:36:26 GMT  
		Size: 490.7 KB (490691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27a9b8a7ecae3c49dde182bd347a2b5af04b62c5736cf281144598fa11632a4`  
		Last Modified: Sat, 20 Jun 2020 00:36:26 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ea38bb9bafeb551f5c0628ea17dca4104b6889dd2d7bc74dcfe5c6e121c691`  
		Last Modified: Sat, 20 Jun 2020 00:36:25 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9747dc4c40e0c137b978ed0deaa10307a09ff3b0bee19e70b28c5b496708ae17`  
		Last Modified: Sat, 20 Jun 2020 00:36:40 GMT  
		Size: 190.5 MB (190469411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb2109b5e65593f432f20cdedc6d27b9b5b3d20ddbb1dc64c76a8f14859528b`  
		Last Modified: Sat, 20 Jun 2020 00:36:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c18a38909760276a17388841a3fbe25a39ec326e654cebf125e834732401c0`  
		Last Modified: Sat, 20 Jun 2020 00:36:23 GMT  
		Size: 662.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed85d81f29ad646a6c4c7580fc53d7c942f7efab5ee6fbec141842831bc8fb08`  
		Last Modified: Sat, 20 Jun 2020 00:36:24 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ba87d5258461fef15e3e285ada8da4b3b861396e9d36cc19be0c5413775c92`  
		Last Modified: Sat, 20 Jun 2020 00:36:24 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8109b8719c0a02345ce49529303bf3d2c05afdbbb4a95f32cd4485246502dc32`  
		Last Modified: Sat, 20 Jun 2020 00:37:54 GMT  
		Size: 719.6 MB (719585456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
