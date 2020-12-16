<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `silverpeas`

-	[`silverpeas:6.0.2`](#silverpeas602)
-	[`silverpeas:6.1.1`](#silverpeas611)
-	[`silverpeas:latest`](#silverpeaslatest)

## `silverpeas:6.0.2`

```console
$ docker pull silverpeas@sha256:b5a456a7a7e5ae6c147e37d1e8968962dd77a477d4d5141e26624edf9e9625ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.0.2` - linux; amd64

```console
$ docker pull silverpeas@sha256:051100ac05b04c8c79febab5e6b6106ecfbf4ca74f7ae35b5bfc1f47249ba4f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1014198284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6acf111b392a8943ac9808d41741a54d0e1e2d21a5b4b9b1d971b9d5069f28a8`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Wed, 25 Nov 2020 22:26:11 GMT
ADD file:8eef54430e581236e6d529a7d09df648f43c840e889d9ae132e5ed25d7bd2b88 in / 
# Wed, 25 Nov 2020 22:26:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:26:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:26:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:26:14 GMT
CMD ["/bin/bash"]
# Wed, 16 Dec 2020 20:18:16 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Wed, 16 Dec 2020 20:18:16 GMT
ENV TERM=xterm
# Wed, 16 Dec 2020 20:21:10 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Wed, 16 Dec 2020 20:21:14 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Wed, 16 Dec 2020 20:21:19 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Wed, 16 Dec 2020 20:21:19 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Wed, 16 Dec 2020 20:21:25 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Wed, 16 Dec 2020 20:21:25 GMT
ENV LANG=en_US.UTF-8
# Wed, 16 Dec 2020 20:21:26 GMT
ENV LANGUAGE=en_US.UTF-8
# Wed, 16 Dec 2020 20:21:26 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 16 Dec 2020 20:21:28 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 16 Dec 2020 20:21:30 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 16 Dec 2020 20:21:30 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 16 Dec 2020 20:21:31 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Wed, 16 Dec 2020 20:21:31 GMT
ENV JBOSS_HOME=/opt/wildfly
# Wed, 16 Dec 2020 20:21:31 GMT
ENV SILVERPEAS_VERSION=6.0.2
# Wed, 16 Dec 2020 20:21:32 GMT
ENV WILDFLY_VERSION=10.1.0
# Wed, 16 Dec 2020 20:21:32 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.0.2 build=1
# Wed, 16 Dec 2020 20:22:49 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Wed, 16 Dec 2020 20:22:50 GMT
COPY file:d12fb4c8fc28235c5621533a9ae0d98ba26e3adf1ffc690da4a6118aa71d8190 in /root/.m2/ 
# Wed, 16 Dec 2020 20:22:50 GMT
WORKDIR /opt/silverpeas/bin
# Wed, 16 Dec 2020 20:22:51 GMT
COPY file:31e3db287bacfa9fb086f2ae49169410b9f0fdf4178bf47d0ebe93621aa996e4 in /opt/ 
# Wed, 16 Dec 2020 20:22:51 GMT
COPY file:5d883339e9add47c37406a038c7747cafede9f81436843206bab5bde7da6e2f6 in /opt/silverpeas/configuration/silverpeas/ 
# Wed, 16 Dec 2020 20:26:56 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas assemble   && rm ../log/build-*   && touch .install
# Wed, 16 Dec 2020 20:26:58 GMT
EXPOSE 8000 9990
# Wed, 16 Dec 2020 20:26:58 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/xmlcomponents/workflows]
# Wed, 16 Dec 2020 20:26:58 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:be8ec4e48d7f24a9a1c01063e5dfabb092c2c1ec73e125113848553c9b07eb8c`  
		Last Modified: Sat, 31 Oct 2020 14:20:23 GMT  
		Size: 45.8 MB (45838270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8b485aff0509bb0fa67dff6a2aa82e9b7b17e5ef28c1673467ec83edb945d`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d887158cc58cbfc3d03cefd5c0b15175fae66ffbf6f28a56180c51cbb5062b8a`  
		Last Modified: Wed, 25 Nov 2020 22:27:14 GMT  
		Size: 533.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05895bb28c18264f614acd13e401b3c5594e12d9fe90d7e52929d3e810e11e97`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24cead373589e581d11688e096f57d8a7d4095bbff2815de5caf5d921626c29`  
		Last Modified: Wed, 16 Dec 2020 20:31:27 GMT  
		Size: 207.4 MB (207390114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e62224d3df03fa20755997297cac6dda83332f2c8e96a784214f21352b721a`  
		Last Modified: Wed, 16 Dec 2020 20:30:15 GMT  
		Size: 4.0 MB (3994029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61953380f7b2798014f8810027b20de5a0230d0979490c9fdcce84c8d7e8bd25`  
		Last Modified: Wed, 16 Dec 2020 20:30:17 GMT  
		Size: 7.1 MB (7146616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6079ceb31c69ee3223376329fc66d5f5f8988cfc460c5388295903cb3f18072`  
		Last Modified: Wed, 16 Dec 2020 20:30:11 GMT  
		Size: 845.4 KB (845417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0b4e7273c79b4dbc59734c9ffa910bdebfc3a906fa646138f0ab660f3253df`  
		Last Modified: Wed, 16 Dec 2020 20:30:10 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef746e564e4438da6ae77a0ef6188cd819449f1a5ea0073437a2a7de2a2caf7c`  
		Last Modified: Wed, 16 Dec 2020 20:30:11 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240cde151e1bd15a592e4f33db27cbf607f57f5d2823187298d39ab90bd3f6f2`  
		Last Modified: Wed, 16 Dec 2020 20:30:33 GMT  
		Size: 144.3 MB (144284551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83571290b017c58dd5febe19f722a1ff999c8f0d4bff17308807cf6c0bf972fa`  
		Last Modified: Wed, 16 Dec 2020 20:30:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1b7ced239e159ccc36751c092a008c9718eb8094290163d19aab480d362f06`  
		Last Modified: Wed, 16 Dec 2020 20:30:09 GMT  
		Size: 809.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325250c37ca8d33369f85596c72755b8bf7ff3e83df054134ac2c10df0b33490`  
		Last Modified: Wed, 16 Dec 2020 20:30:09 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947e08e72cb3f83c64a637568d723b2e69a6349c51e1b1abe5dd18f3ae2fa3ec`  
		Last Modified: Wed, 16 Dec 2020 20:31:30 GMT  
		Size: 604.7 MB (604695767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:6.1.1`

```console
$ docker pull silverpeas@sha256:af96dc8b95d1f9bbe5025f132713235a312baea813d43ab3f868348f67d87a8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:6.1.1` - linux; amd64

```console
$ docker pull silverpeas@sha256:97544137b06abdb25d3a9194907cb258211ea5ba394eacd8a0fd2eda901bb461
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1427266046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:853ed50ce25258c4ebf588a9649a56f57256089b87995d46bbb9ec1b73087370`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Wed, 16 Dec 2020 20:09:21 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Wed, 16 Dec 2020 20:09:21 GMT
ENV TERM=xterm
# Wed, 16 Dec 2020 20:15:19 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Wed, 16 Dec 2020 20:15:23 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Wed, 16 Dec 2020 20:15:27 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Wed, 16 Dec 2020 20:15:27 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Wed, 16 Dec 2020 20:15:33 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Wed, 16 Dec 2020 20:15:33 GMT
ENV LANG=en_US.UTF-8
# Wed, 16 Dec 2020 20:15:33 GMT
ENV LANGUAGE=en_US.UTF-8
# Wed, 16 Dec 2020 20:15:34 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 16 Dec 2020 20:15:35 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 16 Dec 2020 20:15:37 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 16 Dec 2020 20:15:37 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 16 Dec 2020 20:15:38 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Wed, 16 Dec 2020 20:15:38 GMT
ENV JBOSS_HOME=/opt/wildfly
# Wed, 16 Dec 2020 20:15:38 GMT
ENV SILVERPEAS_VERSION=6.1.1
# Wed, 16 Dec 2020 20:15:39 GMT
ENV WILDFLY_VERSION=18.0.1
# Wed, 16 Dec 2020 20:15:39 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.1.1 build=1
# Wed, 16 Dec 2020 20:15:54 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Wed, 16 Dec 2020 20:15:54 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Wed, 16 Dec 2020 20:15:55 GMT
WORKDIR /opt/silverpeas/bin
# Wed, 16 Dec 2020 20:15:55 GMT
COPY file:bd0a4d5e9017df7c7d4b9ba1011c737b2e2fcbe0966662e3315fabb5498b8aa3 in /opt/ 
# Wed, 16 Dec 2020 20:15:55 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Wed, 16 Dec 2020 20:18:07 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas construct   && rm ../log/build-*   && touch .install
# Wed, 16 Dec 2020 20:18:08 GMT
EXPOSE 8000 9990
# Wed, 16 Dec 2020 20:18:08 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Wed, 16 Dec 2020 20:18:09 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7073622117a7f20c010999b974041f73943817eb32926609ceb459fe948b6c49`  
		Last Modified: Wed, 16 Dec 2020 20:29:50 GMT  
		Size: 482.2 MB (482185522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6966b2df5cf7ce8f61dffb23818162a1468e7e60cf3d0cf261cf2be718104334`  
		Last Modified: Wed, 16 Dec 2020 20:27:24 GMT  
		Size: 4.0 MB (3994026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c452167ca7eb436a681cf8b1c569710e32e8e318bfe861c29445a39806e393b`  
		Last Modified: Wed, 16 Dec 2020 20:27:24 GMT  
		Size: 7.1 MB (7146630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0880867eb020aa408463480d42ef8558ec2b145d63456cef1bee5a412954be`  
		Last Modified: Wed, 16 Dec 2020 20:27:20 GMT  
		Size: 490.7 KB (490687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e89e366b0bb98beb5792e7785e34d77252e74e06be6226374030bb0b9f074f`  
		Last Modified: Wed, 16 Dec 2020 20:27:18 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50eabe4b7841fd3de0267dd0e31c9628846377d17295a68b4b3e09f08a4493c`  
		Last Modified: Wed, 16 Dec 2020 20:27:18 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49aa064fab20a8b48c151543d060195cd921c201af68090532689b7dd87650f`  
		Last Modified: Wed, 16 Dec 2020 20:27:48 GMT  
		Size: 190.5 MB (190469061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ff37cbe8cccc4493ffe0a0f1b00751bb2718709a8803317fe6571ff08569c4`  
		Last Modified: Wed, 16 Dec 2020 20:27:17 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e200f65987e59f83564e2bc552402f8ed3d322d3ad23a3b42fc8eb723132eb`  
		Last Modified: Wed, 16 Dec 2020 20:27:17 GMT  
		Size: 761.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f82fed1c972f2f3596ba78c165b026fe108dc5a24427facbdec2522f6fdaaf0`  
		Last Modified: Wed, 16 Dec 2020 20:27:17 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574b1f50fc3c789fd38b6319eb99d85a88ba98398f1dec95cea554bd83b09c25`  
		Last Modified: Wed, 16 Dec 2020 20:28:57 GMT  
		Size: 716.3 MB (716269129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `silverpeas:latest`

```console
$ docker pull silverpeas@sha256:af96dc8b95d1f9bbe5025f132713235a312baea813d43ab3f868348f67d87a8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `silverpeas:latest` - linux; amd64

```console
$ docker pull silverpeas@sha256:97544137b06abdb25d3a9194907cb258211ea5ba394eacd8a0fd2eda901bb461
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1427266046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:853ed50ce25258c4ebf588a9649a56f57256089b87995d46bbb9ec1b73087370`
-	Default Command: `["\/opt\/run.sh"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Wed, 16 Dec 2020 20:09:21 GMT
MAINTAINER Miguel Moquillon "miguel.moquillon@silverpeas.org"
# Wed, 16 Dec 2020 20:09:21 GMT
ENV TERM=xterm
# Wed, 16 Dec 2020 20:15:19 GMT
RUN apt-get update && apt-get install -y     wget     locales     procps     net-tools     zip     unzip     openjdk-8-jdk     ffmpeg     imagemagick     ghostscript     libreoffice     ure     gpgv   && rm -rf /var/lib/apt/lists/*   && update-ca-certificates -f
# Wed, 16 Dec 2020 20:15:23 GMT
RUN wget -nc https://www.silverpeas.org/files/swftools-bin-0.9.2.zip   && echo 'd40bd091c84bde2872f2733a3c767b3a686c8e8477a3af3a96ef347cf05c5e43 *swftools-bin-0.9.2.zip' | sha256sum -   && unzip swftools-bin-0.9.2.zip -d /   && rm swftools-bin-0.9.2.zip
# Wed, 16 Dec 2020 20:15:27 GMT
RUN wget -nc https://www.silverpeas.org/files/pdf2json-bin-0.68.zip   && echo 'eec849cdd75224f9d44c0999ed1fbe8764a773d8ab0cf7fff4bf922ab81c9f84 *pdf2json-bin-0.68.zip' | sha256sum -   && unzip pdf2json-bin-0.68.zip -d /   && rm pdf2json-bin-0.68.zip
# Wed, 16 Dec 2020 20:15:27 GMT
ARG DEFAULT_LOCALE=en_US.UTF-8
# Wed, 16 Dec 2020 20:15:33 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen   && echo "fr_FR.UTF-8 UTF-8" >> /etc/locale.gen   && echo "de_DE.UTF-8 UTF-8" >> /etc/locale.gen   && locale-gen   && update-locale LANG=${DEFAULT_LOCALE} LANGUAGE=${DEFAULT_LOCALE} LC_ALL=${DEFAULT_LOCALE}
# Wed, 16 Dec 2020 20:15:33 GMT
ENV LANG=en_US.UTF-8
# Wed, 16 Dec 2020 20:15:33 GMT
ENV LANGUAGE=en_US.UTF-8
# Wed, 16 Dec 2020 20:15:34 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 16 Dec 2020 20:15:35 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 16 Dec 2020 20:15:37 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 16 Dec 2020 20:15:37 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 16 Dec 2020 20:15:38 GMT
ENV SILVERPEAS_HOME=/opt/silverpeas
# Wed, 16 Dec 2020 20:15:38 GMT
ENV JBOSS_HOME=/opt/wildfly
# Wed, 16 Dec 2020 20:15:38 GMT
ENV SILVERPEAS_VERSION=6.1.1
# Wed, 16 Dec 2020 20:15:39 GMT
ENV WILDFLY_VERSION=18.0.1
# Wed, 16 Dec 2020 20:15:39 GMT
LABEL name=Silverpeas 6 description=Image to install and to run Silverpeas 6 vendor=Silverpeas version=6.1.1 build=1
# Wed, 16 Dec 2020 20:15:54 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc https://www.silverpeas.org/files/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 3F4657EF9C591F2FEA458FEBC19391EB3DF442B6   && gpg --batch --verify silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip.asc silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip   && wget -nc http://download.jboss.org/wildfly/${WILDFLY_VERSION}.Final/wildfly-${WILDFLY_VERSION}.Final.zip   && unzip silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?}.zip -d /opt   && unzip wildfly-${WILDFLY_VERSION}.Final.zip -d /opt   && mv /opt/silverpeas-${SILVERPEAS_VERSION}-wildfly${WILDFLY_VERSION%.?.?} /opt/silverpeas   && mv /opt/wildfly-${WILDFLY_VERSION}.Final /opt/wildfly   && rm *.zip   && mkdir -p /root/.m2
# Wed, 16 Dec 2020 20:15:54 GMT
COPY file:4d0e637a3e1ce0b8143795fd5df1997a7ee18fba27382849ed23e9ecb8142009 in /root/.m2/ 
# Wed, 16 Dec 2020 20:15:55 GMT
WORKDIR /opt/silverpeas/bin
# Wed, 16 Dec 2020 20:15:55 GMT
COPY file:bd0a4d5e9017df7c7d4b9ba1011c737b2e2fcbe0966662e3315fabb5498b8aa3 in /opt/ 
# Wed, 16 Dec 2020 20:15:55 GMT
COPY file:b5a807d0a061fd9e87c6acfc7080c110a5f3c030251fe9a4c995cec7603e12d2 in /opt/silverpeas/configuration/silverpeas/ 
# Wed, 16 Dec 2020 20:18:07 GMT
# ARGS: DEFAULT_LOCALE=en_US.UTF-8
RUN ./silverpeas construct   && rm ../log/build-*   && touch .install
# Wed, 16 Dec 2020 20:18:08 GMT
EXPOSE 8000 9990
# Wed, 16 Dec 2020 20:18:08 GMT
VOLUME [/opt/silverpeas/log /opt/silverpeas/data /opt/silverpeas/properties /opt/silverpeas/xmlcomponents/workflows]
# Wed, 16 Dec 2020 20:18:09 GMT
CMD ["/opt/run.sh"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7073622117a7f20c010999b974041f73943817eb32926609ceb459fe948b6c49`  
		Last Modified: Wed, 16 Dec 2020 20:29:50 GMT  
		Size: 482.2 MB (482185522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6966b2df5cf7ce8f61dffb23818162a1468e7e60cf3d0cf261cf2be718104334`  
		Last Modified: Wed, 16 Dec 2020 20:27:24 GMT  
		Size: 4.0 MB (3994026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c452167ca7eb436a681cf8b1c569710e32e8e318bfe861c29445a39806e393b`  
		Last Modified: Wed, 16 Dec 2020 20:27:24 GMT  
		Size: 7.1 MB (7146630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0880867eb020aa408463480d42ef8558ec2b145d63456cef1bee5a412954be`  
		Last Modified: Wed, 16 Dec 2020 20:27:20 GMT  
		Size: 490.7 KB (490687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e89e366b0bb98beb5792e7785e34d77252e74e06be6226374030bb0b9f074f`  
		Last Modified: Wed, 16 Dec 2020 20:27:18 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50eabe4b7841fd3de0267dd0e31c9628846377d17295a68b4b3e09f08a4493c`  
		Last Modified: Wed, 16 Dec 2020 20:27:18 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49aa064fab20a8b48c151543d060195cd921c201af68090532689b7dd87650f`  
		Last Modified: Wed, 16 Dec 2020 20:27:48 GMT  
		Size: 190.5 MB (190469061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ff37cbe8cccc4493ffe0a0f1b00751bb2718709a8803317fe6571ff08569c4`  
		Last Modified: Wed, 16 Dec 2020 20:27:17 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e200f65987e59f83564e2bc552402f8ed3d322d3ad23a3b42fc8eb723132eb`  
		Last Modified: Wed, 16 Dec 2020 20:27:17 GMT  
		Size: 761.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f82fed1c972f2f3596ba78c165b026fe108dc5a24427facbdec2522f6fdaaf0`  
		Last Modified: Wed, 16 Dec 2020 20:27:17 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574b1f50fc3c789fd38b6319eb99d85a88ba98398f1dec95cea554bd83b09c25`  
		Last Modified: Wed, 16 Dec 2020 20:28:57 GMT  
		Size: 716.3 MB (716269129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
