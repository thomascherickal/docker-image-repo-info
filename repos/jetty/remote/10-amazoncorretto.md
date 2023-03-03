## `jetty:10-amazoncorretto`

```console
$ docker pull jetty@sha256:e2ce3d1157737c664ed6d50a1bf483391a903ca94f4918d25f92506571b06cd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:10-amazoncorretto` - linux; amd64

```console
$ docker pull jetty@sha256:4ec1e09eb4e0767f14a76b0f5c789a6e36360daa12d462a4fb5d0165d6ec10d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.2 MB (231233226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c983c5c032b4ae35741c1242c7af46be69e4298a50b30b9d2f0218dbaf2145ea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 02 Mar 2023 22:19:50 GMT
COPY dir:d2afcd884fd8e8edf2c9d3cff550c5573438d40a5b14c0bcde9ea94f2fad31f9 in / 
# Thu, 02 Mar 2023 22:19:51 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 23:19:05 GMT
ARG version=17.0.6.10-1
# Thu, 02 Mar 2023 23:19:34 GMT
# ARGS: version=17.0.6.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 02 Mar 2023 23:19:35 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 23:19:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Fri, 03 Mar 2023 00:04:27 GMT
ENV JETTY_VERSION=10.0.13
# Fri, 03 Mar 2023 00:04:28 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 03 Mar 2023 00:04:28 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 03 Mar 2023 00:04:28 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 03 Mar 2023 00:04:28 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Mar 2023 00:04:28 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.13/jetty-home-10.0.13.tar.gz
# Fri, 03 Mar 2023 00:04:28 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 03 Mar 2023 00:04:47 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 03 Mar 2023 00:04:48 GMT
WORKDIR /var/lib/jetty
# Fri, 03 Mar 2023 00:04:48 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Fri, 03 Mar 2023 00:04:48 GMT
USER jetty
# Fri, 03 Mar 2023 00:04:48 GMT
EXPOSE 8080
# Fri, 03 Mar 2023 00:04:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 03 Mar 2023 00:04:48 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:65e7c8d35fc567b9f18bb2fe2de2c278d644adafea6fc7487a3a40d8693ef6dc`  
		Last Modified: Tue, 28 Feb 2023 20:08:25 GMT  
		Size: 62.4 MB (62389508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8675c8198162c00951d3d53a075ffb6632b0afb15d4154e2f46571e0e2a99a82`  
		Last Modified: Thu, 02 Mar 2023 23:23:41 GMT  
		Size: 152.0 MB (151953486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fb681f114ce6b63050ea5245f4cf5994f599ef97460567b96b74efb0d685e9`  
		Last Modified: Fri, 03 Mar 2023 00:10:44 GMT  
		Size: 16.9 MB (16888792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60c61c741366d6419b1df056ff135c470bf40d2f0e354976094cf497364c17c`  
		Last Modified: Fri, 03 Mar 2023 00:10:42 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:10-amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:9236e17bc6e9d8e44191389d0ff99ec46a751abb912e161f4656f58d4e7288b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.4 MB (231428825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777c074bdc68f8c1e8ae99c954ff07cfab66e0d91c3ccb0556c326c0e7ac4db8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 02 Mar 2023 22:39:28 GMT
COPY dir:82034448b19235d709c5681caa8414343fb6e1711c03e26721c451fa22d139eb in / 
# Thu, 02 Mar 2023 22:39:28 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 23:49:02 GMT
ARG version=17.0.6.10-1
# Thu, 02 Mar 2023 23:49:22 GMT
# ARGS: version=17.0.6.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 02 Mar 2023 23:49:23 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 23:49:23 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Fri, 03 Mar 2023 00:25:56 GMT
ENV JETTY_VERSION=10.0.13
# Fri, 03 Mar 2023 00:25:56 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 03 Mar 2023 00:25:57 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 03 Mar 2023 00:25:57 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 03 Mar 2023 00:25:57 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Mar 2023 00:25:57 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.13/jetty-home-10.0.13.tar.gz
# Fri, 03 Mar 2023 00:25:57 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 03 Mar 2023 00:26:13 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 03 Mar 2023 00:26:13 GMT
WORKDIR /var/lib/jetty
# Fri, 03 Mar 2023 00:26:14 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Fri, 03 Mar 2023 00:26:14 GMT
USER jetty
# Fri, 03 Mar 2023 00:26:14 GMT
EXPOSE 8080
# Fri, 03 Mar 2023 00:26:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 03 Mar 2023 00:26:14 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:ff7a305ba0c9eeef6825ac8bbba292756a82e85d36e370fc6294d9b7cf402a6b`  
		Last Modified: Wed, 01 Mar 2023 07:58:02 GMT  
		Size: 64.0 MB (63999614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2621c082ed529526d3b8aa96a2cddfaf8443d77c6737d417c1c30807f9c981ac`  
		Last Modified: Thu, 02 Mar 2023 23:51:43 GMT  
		Size: 150.5 MB (150489185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f061c0b236ac6f30f162c266b95d8d407c52a739fc02d67012e69ba42c321edf`  
		Last Modified: Fri, 03 Mar 2023 00:30:25 GMT  
		Size: 16.9 MB (16938585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6430dac8da6526725a5f79e6c5215f5380ed9dbbcd4f65dab0432c3581c47e4`  
		Last Modified: Fri, 03 Mar 2023 00:30:23 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
