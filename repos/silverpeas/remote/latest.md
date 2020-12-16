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
