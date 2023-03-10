## `jetty:10-jdk17-amazoncorretto`

```console
$ docker pull jetty@sha256:2ba6f92e893ab6478603bc13cafdbb2d7e30e8043722ff0cef20203c73668ab1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:10-jdk17-amazoncorretto` - linux; amd64

```console
$ docker pull jetty@sha256:cfb80b07b9123c05099a2007cd6786de4a4cfb92106999b8da5362346dba9f16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.3 MB (231300223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b6a5f7f669195b8d41b05d70c9eaeb5639fd2aa8e71a66d315830f362e42f66`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Fri, 10 Mar 2023 01:20:24 GMT
COPY dir:1fe253a28ffa7545ac05b2d6b2410c0b48083e8195b6557287b6a94e845122d3 in / 
# Fri, 10 Mar 2023 01:20:24 GMT
CMD ["/bin/bash"]
# Fri, 10 Mar 2023 01:39:37 GMT
ARG version=17.0.6.10-1
# Fri, 10 Mar 2023 01:40:01 GMT
# ARGS: version=17.0.6.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 10 Mar 2023 01:40:02 GMT
ENV LANG=C.UTF-8
# Fri, 10 Mar 2023 01:40:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Fri, 10 Mar 2023 02:25:12 GMT
ENV JETTY_VERSION=10.0.13
# Fri, 10 Mar 2023 02:25:12 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 10 Mar 2023 02:25:12 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 10 Mar 2023 02:25:12 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 10 Mar 2023 02:25:12 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Mar 2023 02:25:12 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.13/jetty-home-10.0.13.tar.gz
# Fri, 10 Mar 2023 02:25:12 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 10 Mar 2023 02:25:30 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 10 Mar 2023 02:25:30 GMT
WORKDIR /var/lib/jetty
# Fri, 10 Mar 2023 02:25:31 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Fri, 10 Mar 2023 02:25:31 GMT
USER jetty
# Fri, 10 Mar 2023 02:25:31 GMT
EXPOSE 8080
# Fri, 10 Mar 2023 02:25:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 02:25:31 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:07e4d356f367b468402d36db62e60b734522576ce93a8e7246f1b36899c58f5e`  
		Last Modified: Thu, 09 Mar 2023 17:52:43 GMT  
		Size: 62.5 MB (62477005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc5c757e99e469625f77245de910e479c38b27e19879a86152769c49de9368f`  
		Last Modified: Fri, 10 Mar 2023 01:44:45 GMT  
		Size: 151.9 MB (151943959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238f43fab13140ef10bae4cdc1339bff28bd412bd33f27b5d09dcfeb70d7abf0`  
		Last Modified: Fri, 10 Mar 2023 02:31:58 GMT  
		Size: 16.9 MB (16877819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa673e21652a62403fcde580794ceac1e215720256da87bb58bce20a057c8c3`  
		Last Modified: Fri, 10 Mar 2023 02:31:57 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:10-jdk17-amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:180e4f131ff085c7277fb99abe61d77a8c5c9b08858ef573cd0cf7f66e499eb5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231569666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c2d86b739ddd220deb2d2475c26607faacf7100a1a11727d383cd5d3634ae92`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Fri, 10 Mar 2023 01:39:35 GMT
COPY dir:1997e4057e1f8b7df06806432d2b2c303c1f6ef5b18e8273d4393b867415d8b2 in / 
# Fri, 10 Mar 2023 01:39:36 GMT
CMD ["/bin/bash"]
# Fri, 10 Mar 2023 02:04:07 GMT
ARG version=17.0.6.10-1
# Fri, 10 Mar 2023 02:04:26 GMT
# ARGS: version=17.0.6.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 10 Mar 2023 02:04:28 GMT
ENV LANG=C.UTF-8
# Fri, 10 Mar 2023 02:04:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Fri, 10 Mar 2023 02:40:34 GMT
ENV JETTY_VERSION=10.0.13
# Fri, 10 Mar 2023 02:40:34 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 10 Mar 2023 02:40:34 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 10 Mar 2023 02:40:34 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 10 Mar 2023 02:40:35 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Mar 2023 02:40:35 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.13/jetty-home-10.0.13.tar.gz
# Fri, 10 Mar 2023 02:40:35 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 10 Mar 2023 02:40:49 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 10 Mar 2023 02:40:50 GMT
WORKDIR /var/lib/jetty
# Fri, 10 Mar 2023 02:40:50 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Fri, 10 Mar 2023 02:40:50 GMT
USER jetty
# Fri, 10 Mar 2023 02:40:50 GMT
EXPOSE 8080
# Fri, 10 Mar 2023 02:40:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 02:40:50 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:042c9cfa8a36c0ffe86667a7dd7d488f78cbe295aa845213c01fdf8784165a92`  
		Last Modified: Fri, 10 Mar 2023 01:40:11 GMT  
		Size: 64.1 MB (64125204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4067f688859ee360de86915e59b24d2de2e1628f042940c7e1106369a9203e47`  
		Last Modified: Fri, 10 Mar 2023 02:06:38 GMT  
		Size: 150.5 MB (150491225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfad76f4673a02266f79b66228a1bcceca20b9da9d75d7b3b085e4b876981a1`  
		Last Modified: Fri, 10 Mar 2023 02:45:04 GMT  
		Size: 17.0 MB (16951795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5e0f04f48d35c4300564329fc02c8ae5998f29792b5357a6e0e70214d4c476`  
		Last Modified: Fri, 10 Mar 2023 02:45:03 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
