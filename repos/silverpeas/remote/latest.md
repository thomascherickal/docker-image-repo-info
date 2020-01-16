## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:6504440335c3434f3fd07f7b7295fcdcfcf16449110743676da65a72a8f4a755
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:e2474dd1925dc9d534ee9c3d3a13e71c32875adccdd0c69d3c8aea22e0f17429
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1011306694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79b6eaa9a7c3c1d29b7369524a5ce9e88aeffb164d2598b61334da448708c594`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:54:34 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Thu, 16 Jan 2020 02:54:34 GMT
ENV TERM=xterm
# Thu, 16 Jan 2020 02:56:17 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Thu, 16 Jan 2020 02:56:20 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Thu, 16 Jan 2020 02:56:22 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Thu, 16 Jan 2020 02:56:22 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Thu, 16 Jan 2020 02:56:25 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Thu, 16 Jan 2020 02:56:25 GMT
ENV LANG=en_US.UTF-8
# Thu, 16 Jan 2020 02:56:25 GMT
ENV LANGUAGE=en_US.UTF-8
# Thu, 16 Jan 2020 02:56:25 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 16 Jan 2020 02:56:26 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 16 Jan 2020 02:56:27 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 16 Jan 2020 02:56:27 GMT
ENV JAVA_HOME=/docker-java-home
# Thu, 16 Jan 2020 02:56:27 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Thu, 16 Jan 2020 02:56:27 GMT
ENV JBOSS_HOME=/opt/wildfly
# Thu, 16 Jan 2020 02:56:27 GMT
ENV SILVERPEAS_VERSION=6.0.2
# Thu, 16 Jan 2020 02:56:28 GMT
ENV WILDFLY_VERSION=10.1.0
# Thu, 16 Jan 2020 02:56:28 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.0.2 build=1
# Thu, 16 Jan 2020 02:56:42 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Thu, 16 Jan 2020 02:56:42 GMT
COPY file:d12fb4c8fc28235c5621533a9ae0d98ba26e3adf1ffc690da4a6118aa71d8190 in /root/.m2/ 
# Thu, 16 Jan 2020 02:56:42 GMT
WORKDIR /opt/silverpeas/bin
# Thu, 16 Jan 2020 02:56:43 GMT
COPY file:31e3db287bacfa9fb086f2ae49169410b9f0fdf4178bf47d0ebe93621aa996e4 in /opt/ 
# Thu, 16 Jan 2020 02:56:43 GMT
COPY file:5d883339e9add47c37406a038c7747cafede9f81436843206bab5bde7da6e2f6 in /opt/silverpeas/configuration/silverpeas/ 
# Thu, 16 Jan 2020 03:01:04 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas assemble   && rm ../log/build-*   && touch .install
# Thu, 16 Jan 2020 03:01:05 GMT
EXPOSE 8000 9990
# Thu, 16 Jan 2020 03:01:05 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/xmlcomponents/workflows]
# Thu, 16 Jan 2020 03:01:05 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfab7e52b68afbc184b0802915e982282eadf15a0572dcbc0e1a24c16da4341e`  
		Last Modified: Thu, 16 Jan 2020 03:02:04 GMT  
		Size: 206.2 MB (206187280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64882e2595eaa0583d1aeea74f675c0bf74624e206c42514eaf99c8cbbb1067e`  
		Last Modified: Thu, 16 Jan 2020 03:01:29 GMT  
		Size: 4.0 MB (3994027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74d17eed7b245e5dd834f5d7fd0ad579290785f4d64208b13d415511ef08643`  
		Last Modified: Thu, 16 Jan 2020 03:01:29 GMT  
		Size: 7.1 MB (7146612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6881a3cc51cbb737ef03e321e9985559f8b2bf14f3f1cc500e9b8c19c7b845`  
		Last Modified: Thu, 16 Jan 2020 03:01:27 GMT  
		Size: 845.4 KB (845399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2c61d18ed7bd96fd3b16ad334de9d1d657821838ae53cb3080480627ef3597`  
		Last Modified: Thu, 16 Jan 2020 03:01:27 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4652ea1912c80a354915c918d703225e26f94df82f226b6668b3a336479953`  
		Last Modified: Thu, 16 Jan 2020 03:01:27 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08da69c160ba4843654a8b8b7b24eacc8bdd325832fc0d1608747dccdf63fdf`  
		Last Modified: Thu, 16 Jan 2020 03:01:56 GMT  
		Size: 144.3 MB (144284498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d604633bde068d883918e3cff736630522a5171dcd37a84c6e0c500850173f`  
		Last Modified: Thu, 16 Jan 2020 03:01:25 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d402264f5ff44a4b0e9da881ed02bb51d1cddc9bdcc9a1c54b1b26d0e3e33d7b`  
		Last Modified: Thu, 16 Jan 2020 03:01:25 GMT  
		Size: 805.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84160e6cd15f50ab2cd4f74866773a2c5e1c6a07430df90cff0730943b8e4d5c`  
		Last Modified: Thu, 16 Jan 2020 03:01:25 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ced680bba47411a38d370c70027096ff4b24970d52f061c12422025555cdcd`  
		Last Modified: Thu, 16 Jan 2020 03:02:07 GMT  
		Size: 604.7 MB (604695622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
