## `jetty:10-jdk11-amazoncorretto`

```console
$ docker pull jetty@sha256:db7adf78e4880dee1fcc5f183e0c767b3e21c3c5fc79cbd0d2cc6cf921465bfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:10-jdk11-amazoncorretto` - linux; amd64

```console
$ docker pull jetty@sha256:f727fe2d8be8c2d68acd9394293cdb7b5d5538a21059fa7d548b8e945445caf6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.1 MB (227067836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e5930ba3c7b24a5e5c2914b7b89c8c5555c6f7c2423d7279bd4ce5ee30f8551`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 02 Mar 2023 22:19:50 GMT
COPY dir:d2afcd884fd8e8edf2c9d3cff550c5573438d40a5b14c0bcde9ea94f2fad31f9 in / 
# Thu, 02 Mar 2023 22:19:51 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 23:18:17 GMT
ARG version=11.0.18.10-1
# Thu, 02 Mar 2023 23:18:45 GMT
# ARGS: version=11.0.18.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 02 Mar 2023 23:18:46 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 23:18:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Fri, 03 Mar 2023 00:04:53 GMT
ENV JETTY_VERSION=10.0.13
# Fri, 03 Mar 2023 00:04:53 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 03 Mar 2023 00:04:53 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 03 Mar 2023 00:04:53 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 03 Mar 2023 00:04:54 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Mar 2023 00:04:54 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.13/jetty-home-10.0.13.tar.gz
# Fri, 03 Mar 2023 00:04:54 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 03 Mar 2023 00:05:14 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 03 Mar 2023 00:05:14 GMT
WORKDIR /var/lib/jetty
# Fri, 03 Mar 2023 00:05:14 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Fri, 03 Mar 2023 00:05:14 GMT
USER jetty
# Fri, 03 Mar 2023 00:05:14 GMT
EXPOSE 8080
# Fri, 03 Mar 2023 00:05:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 03 Mar 2023 00:05:14 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:65e7c8d35fc567b9f18bb2fe2de2c278d644adafea6fc7487a3a40d8693ef6dc`  
		Last Modified: Tue, 28 Feb 2023 20:08:25 GMT  
		Size: 62.4 MB (62389508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4cbd53f77ac6bf584b8802e92397dfd8961b19face024ecf7771e152445b94`  
		Last Modified: Thu, 02 Mar 2023 23:23:03 GMT  
		Size: 147.8 MB (147790063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7bbb2bee159abdf7e8be85506e2659387530a1e171c071a90fea1a7278d200`  
		Last Modified: Fri, 03 Mar 2023 00:11:03 GMT  
		Size: 16.9 MB (16886825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19edb5072f5af54d2c528d4604e17afa50b1f49b9a16af70cdb8f6fc80e9230a`  
		Last Modified: Fri, 03 Mar 2023 00:11:01 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:10-jdk11-amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:260813498c256f9a20b7a7d9d26ff7e3d533cf9e5cd0d71d9a6d30071ee6ec0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.9 MB (225881773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9a9654764c904c4ad8221db66e6a2ecddc4e5034eae8d0a3085e069e9879bb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 02 Mar 2023 22:39:28 GMT
COPY dir:82034448b19235d709c5681caa8414343fb6e1711c03e26721c451fa22d139eb in / 
# Thu, 02 Mar 2023 22:39:28 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 23:48:33 GMT
ARG version=11.0.18.10-1
# Thu, 02 Mar 2023 23:48:52 GMT
# ARGS: version=11.0.18.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 02 Mar 2023 23:48:54 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 23:48:54 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Fri, 03 Mar 2023 00:26:16 GMT
ENV JETTY_VERSION=10.0.13
# Fri, 03 Mar 2023 00:26:16 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 03 Mar 2023 00:26:16 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 03 Mar 2023 00:26:16 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 03 Mar 2023 00:26:16 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Mar 2023 00:26:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.13/jetty-home-10.0.13.tar.gz
# Fri, 03 Mar 2023 00:26:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 03 Mar 2023 00:26:32 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 03 Mar 2023 00:26:33 GMT
WORKDIR /var/lib/jetty
# Fri, 03 Mar 2023 00:26:33 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Fri, 03 Mar 2023 00:26:33 GMT
USER jetty
# Fri, 03 Mar 2023 00:26:33 GMT
EXPOSE 8080
# Fri, 03 Mar 2023 00:26:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 03 Mar 2023 00:26:33 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:ff7a305ba0c9eeef6825ac8bbba292756a82e85d36e370fc6294d9b7cf402a6b`  
		Last Modified: Wed, 01 Mar 2023 07:58:02 GMT  
		Size: 64.0 MB (63999614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddebac930d792daa64670c6e89a4a9e003d63098dd1bbbc29a0d1b50f929ab8`  
		Last Modified: Thu, 02 Mar 2023 23:51:12 GMT  
		Size: 145.0 MB (144952168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c738f502a48281e4a92e01cfa57bb7dd7884925e733a1b728bbca7a7b22124c8`  
		Last Modified: Fri, 03 Mar 2023 00:30:42 GMT  
		Size: 16.9 MB (16928550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb3f7d208ef7dd65fd6ec282134277be16081bdf16fb7b274d01c82dfb7a874`  
		Last Modified: Fri, 03 Mar 2023 00:30:41 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
