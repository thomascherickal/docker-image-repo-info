## `jetty:11-jdk17-amazoncorretto`

```console
$ docker pull jetty@sha256:6f0de6830f76b93cff02f9a86eeb9a2ef356df2af6be9749320d2c93643d5cca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:11-jdk17-amazoncorretto` - linux; amd64

```console
$ docker pull jetty@sha256:8e66f8f13e687d666c7a4e3f2796ce2d299270885698463aff86c098b6ba5cb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.7 MB (234730066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84f6bb9783c912e62b0f036500cfd9d54f02d8efbc86ec9d791b7f38022dae48`
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
# Fri, 03 Mar 2023 00:03:35 GMT
ENV JETTY_VERSION=11.0.13
# Fri, 03 Mar 2023 00:03:36 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 03 Mar 2023 00:03:36 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 03 Mar 2023 00:03:36 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 03 Mar 2023 00:03:36 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Mar 2023 00:03:36 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/11.0.13/jetty-home-11.0.13.tar.gz
# Fri, 03 Mar 2023 00:03:36 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 03 Mar 2023 00:03:55 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 03 Mar 2023 00:03:56 GMT
WORKDIR /var/lib/jetty
# Fri, 03 Mar 2023 00:03:56 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Fri, 03 Mar 2023 00:03:56 GMT
USER jetty
# Fri, 03 Mar 2023 00:03:56 GMT
EXPOSE 8080
# Fri, 03 Mar 2023 00:03:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 03 Mar 2023 00:03:56 GMT
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
	-	`sha256:9a08d59d1ef68b39fe35dd7587aa14f376154e4b9df4ef1af3d869105184a1e9`  
		Last Modified: Fri, 03 Mar 2023 00:10:11 GMT  
		Size: 20.4 MB (20385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8ca927bcadae6397cda8f06a3a5361939eb8ce8bc653d4ffdfa32bde2ac155`  
		Last Modified: Fri, 03 Mar 2023 00:10:10 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:11-jdk17-amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:1bbb1d7c355ea128f4437402575cc37990dcc3c966a00a9234147ba1ac0843a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234923433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:017db337ec053204962bbba4a7325c1342c2975658966e19dbc51bcc5efcd1c1`
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
# Fri, 03 Mar 2023 00:25:17 GMT
ENV JETTY_VERSION=11.0.13
# Fri, 03 Mar 2023 00:25:18 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 03 Mar 2023 00:25:18 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 03 Mar 2023 00:25:18 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 03 Mar 2023 00:25:18 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Mar 2023 00:25:18 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/11.0.13/jetty-home-11.0.13.tar.gz
# Fri, 03 Mar 2023 00:25:18 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 03 Mar 2023 00:25:34 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 03 Mar 2023 00:25:34 GMT
WORKDIR /var/lib/jetty
# Fri, 03 Mar 2023 00:25:34 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Fri, 03 Mar 2023 00:25:34 GMT
USER jetty
# Fri, 03 Mar 2023 00:25:34 GMT
EXPOSE 8080
# Fri, 03 Mar 2023 00:25:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 03 Mar 2023 00:25:34 GMT
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
	-	`sha256:4cc0994b681f86a8d8686a5574edd3420e7806cc09a8b9e22991846776a2d353`  
		Last Modified: Fri, 03 Mar 2023 00:29:54 GMT  
		Size: 20.4 MB (20433193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5c1024cc706b4cf7c7b3c8845ecdad3e43fa3bd40b8b21c9e1722ffc58d80f`  
		Last Modified: Fri, 03 Mar 2023 00:29:53 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
