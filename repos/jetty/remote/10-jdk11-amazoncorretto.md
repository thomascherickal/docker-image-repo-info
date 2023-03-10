## `jetty:10-jdk11-amazoncorretto`

```console
$ docker pull jetty@sha256:d14458eb14697a50c346d4315fe4c26b4a828bbc4e0f8f0c8471880457276422
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:10-jdk11-amazoncorretto` - linux; amd64

```console
$ docker pull jetty@sha256:b4d9f382e8572dc40b86020f3c164e097ab0e9d7f2048b61a964490cada2ece0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227153187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:175b642d08f684e202e068f94244efadeece7fddb2db2e985c3bf06d7780c5ea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Fri, 10 Mar 2023 01:20:24 GMT
COPY dir:1fe253a28ffa7545ac05b2d6b2410c0b48083e8195b6557287b6a94e845122d3 in / 
# Fri, 10 Mar 2023 01:20:24 GMT
CMD ["/bin/bash"]
# Fri, 10 Mar 2023 01:38:52 GMT
ARG version=11.0.18.10-1
# Fri, 10 Mar 2023 01:39:16 GMT
# ARGS: version=11.0.18.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 10 Mar 2023 01:39:17 GMT
ENV LANG=C.UTF-8
# Fri, 10 Mar 2023 01:39:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Fri, 10 Mar 2023 02:25:38 GMT
ENV JETTY_VERSION=10.0.13
# Fri, 10 Mar 2023 02:25:38 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 10 Mar 2023 02:25:38 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 10 Mar 2023 02:25:38 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 10 Mar 2023 02:25:38 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Mar 2023 02:25:39 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.13/jetty-home-10.0.13.tar.gz
# Fri, 10 Mar 2023 02:25:39 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 10 Mar 2023 02:25:58 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 10 Mar 2023 02:25:58 GMT
WORKDIR /var/lib/jetty
# Fri, 10 Mar 2023 02:25:58 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Fri, 10 Mar 2023 02:25:58 GMT
USER jetty
# Fri, 10 Mar 2023 02:25:58 GMT
EXPOSE 8080
# Fri, 10 Mar 2023 02:25:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 02:25:58 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:07e4d356f367b468402d36db62e60b734522576ce93a8e7246f1b36899c58f5e`  
		Last Modified: Thu, 09 Mar 2023 17:52:43 GMT  
		Size: 62.5 MB (62477005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138c8f756bf36c956d5822ad40dfcc50eeca12312c0fdd7a3f9255bbd9ec2c2c`  
		Last Modified: Fri, 10 Mar 2023 01:44:08 GMT  
		Size: 147.8 MB (147786051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7468dcfa05e66499a8265245247f410a6ec7b778daa93a06d191c4046b568a4`  
		Last Modified: Fri, 10 Mar 2023 02:32:19 GMT  
		Size: 16.9 MB (16888689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b18f90b71bfb743c07fe3719982d7154d34c4f5e834ed56027d451a41f2db78`  
		Last Modified: Fri, 10 Mar 2023 02:32:17 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:10-jdk11-amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:ad938e33eef5516703bac8d1f16df193870f80b0dc194e3368deadaadc6ce8b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.0 MB (226034184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30fff181b89f57efe54c6fd7dba8caaaa9174554bce66b0f87fcc1871dfd1eb8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Fri, 10 Mar 2023 01:39:35 GMT
COPY dir:1997e4057e1f8b7df06806432d2b2c303c1f6ef5b18e8273d4393b867415d8b2 in / 
# Fri, 10 Mar 2023 01:39:36 GMT
CMD ["/bin/bash"]
# Fri, 10 Mar 2023 02:03:37 GMT
ARG version=11.0.18.10-1
# Fri, 10 Mar 2023 02:03:55 GMT
# ARGS: version=11.0.18.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 10 Mar 2023 02:03:57 GMT
ENV LANG=C.UTF-8
# Fri, 10 Mar 2023 02:03:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Fri, 10 Mar 2023 02:40:54 GMT
ENV JETTY_VERSION=10.0.13
# Fri, 10 Mar 2023 02:40:54 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 10 Mar 2023 02:40:54 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 10 Mar 2023 02:40:54 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 10 Mar 2023 02:40:54 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Mar 2023 02:40:54 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.13/jetty-home-10.0.13.tar.gz
# Fri, 10 Mar 2023 02:40:54 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 10 Mar 2023 02:41:09 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 10 Mar 2023 02:41:09 GMT
WORKDIR /var/lib/jetty
# Fri, 10 Mar 2023 02:41:09 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Fri, 10 Mar 2023 02:41:09 GMT
USER jetty
# Fri, 10 Mar 2023 02:41:09 GMT
EXPOSE 8080
# Fri, 10 Mar 2023 02:41:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 02:41:10 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:042c9cfa8a36c0ffe86667a7dd7d488f78cbe295aa845213c01fdf8784165a92`  
		Last Modified: Fri, 10 Mar 2023 01:40:11 GMT  
		Size: 64.1 MB (64125204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36214bbe9ca13060f6a0953d7f4cbae92f167fcbad49a1548f7f9cedc8ba61e1`  
		Last Modified: Fri, 10 Mar 2023 02:06:09 GMT  
		Size: 145.0 MB (144965229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3239cbe921c59fd6d2a1212250e40ed1772daf582e45078fd6a5085693efc741`  
		Last Modified: Fri, 10 Mar 2023 02:45:22 GMT  
		Size: 16.9 MB (16942311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee5cf3a24d07f6a9466cfad7c93831f5da16a52184826badb5c847d25b2acb0`  
		Last Modified: Fri, 10 Mar 2023 02:45:31 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
