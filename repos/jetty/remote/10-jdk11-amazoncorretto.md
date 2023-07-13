## `jetty:10-jdk11-amazoncorretto`

```console
$ docker pull jetty@sha256:ccd1d20f3a19c5cc7bdeb8132a6347e8f34cccc0228dae49777338b5e62deed4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:10-jdk11-amazoncorretto` - linux; amd64

```console
$ docker pull jetty@sha256:22299701c47483fa3ee8e4354ac9a24b3d758c6799c20ad2e8614ae606237051
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.1 MB (227141195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:560b66d04bfeb01d91d439591b0ae1e257aa7091df0c83b6f4b41e4fb0e66fa3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 13 Jul 2023 01:20:13 GMT
COPY dir:be29c71398840090bec7021ae8f2d354451564507602cf38257ad90a915b1838 in / 
# Thu, 13 Jul 2023 01:20:13 GMT
CMD ["/bin/bash"]
# Thu, 13 Jul 2023 01:39:57 GMT
ARG version=11.0.19.7-1
# Thu, 13 Jul 2023 01:40:20 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 13 Jul 2023 01:40:21 GMT
ENV LANG=C.UTF-8
# Thu, 13 Jul 2023 01:40:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Thu, 13 Jul 2023 02:38:04 GMT
ENV JETTY_VERSION=10.0.15
# Thu, 13 Jul 2023 02:38:04 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 13 Jul 2023 02:38:04 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 13 Jul 2023 02:38:04 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 13 Jul 2023 02:38:04 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Jul 2023 02:38:05 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.15/jetty-home-10.0.15.tar.gz
# Thu, 13 Jul 2023 02:38:05 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Thu, 13 Jul 2023 02:38:23 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 13 Jul 2023 02:38:23 GMT
WORKDIR /var/lib/jetty
# Thu, 13 Jul 2023 02:38:24 GMT
COPY multi:88ca540b9901ef22d614e919524f1d550a54166ea9880b0aa9695f8e0470c8f7 in / 
# Thu, 13 Jul 2023 02:38:24 GMT
USER jetty
# Thu, 13 Jul 2023 02:38:24 GMT
EXPOSE 8080
# Thu, 13 Jul 2023 02:38:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 13 Jul 2023 02:38:24 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e90aa42bc48ff728ab10fd485b42144e863dfd8689dd6ea94c78ac0357ec5101`  
		Last Modified: Fri, 30 Jun 2023 00:09:38 GMT  
		Size: 62.5 MB (62485766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63fa75b5af5d4706a9f75dbd1316dcdaab658d391175348f2edb3fffce66edf`  
		Last Modified: Thu, 13 Jul 2023 01:50:50 GMT  
		Size: 147.8 MB (147801091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb8f4b4886b39e546af5fb0eb1875736b49ee632e6ad585aeeb303e43acd428`  
		Last Modified: Thu, 13 Jul 2023 02:42:46 GMT  
		Size: 16.9 MB (16852725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed5c8cd176b4143dea482c9bb5503f9e669b605bd4fcfceb3370aea89fae13f`  
		Last Modified: Thu, 13 Jul 2023 02:42:45 GMT  
		Size: 1.6 KB (1613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:10-jdk11-amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:2fbb454b518b1144bcf8173a9f7c74fe0d79d534985a47ef97cd82a82c29cdae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.0 MB (225972666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ca2eb3e7aad58ffc892594017a95fe9e180c2f82c705245762de60cfada15c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 13 Jul 2023 00:40:00 GMT
COPY dir:a284fdf4a484ebc9131c665fc151094ec73265d07d353476272944e301722064 in / 
# Thu, 13 Jul 2023 00:40:01 GMT
CMD ["/bin/bash"]
# Thu, 13 Jul 2023 01:05:50 GMT
ARG version=11.0.19.7-1
# Thu, 13 Jul 2023 01:06:08 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 13 Jul 2023 01:06:10 GMT
ENV LANG=C.UTF-8
# Thu, 13 Jul 2023 01:06:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Thu, 13 Jul 2023 01:40:07 GMT
ENV JETTY_VERSION=10.0.15
# Thu, 13 Jul 2023 01:40:07 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 13 Jul 2023 01:40:07 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 13 Jul 2023 01:40:07 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 13 Jul 2023 01:40:07 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Jul 2023 01:40:07 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.15/jetty-home-10.0.15.tar.gz
# Thu, 13 Jul 2023 01:40:07 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Thu, 13 Jul 2023 01:40:22 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 13 Jul 2023 01:40:22 GMT
WORKDIR /var/lib/jetty
# Thu, 13 Jul 2023 01:40:22 GMT
COPY multi:88ca540b9901ef22d614e919524f1d550a54166ea9880b0aa9695f8e0470c8f7 in / 
# Thu, 13 Jul 2023 01:40:22 GMT
USER jetty
# Thu, 13 Jul 2023 01:40:22 GMT
EXPOSE 8080
# Thu, 13 Jul 2023 01:40:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 13 Jul 2023 01:40:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:20c8bca6ae5daad56b485a4b6f1f395a51727d69eb6a7566c53b00a366e46576`  
		Last Modified: Fri, 30 Jun 2023 17:38:06 GMT  
		Size: 64.1 MB (64128925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e87f9acff5208a6ce4c1bdad3e641eb5b5e28d07ee04e786a5d7b24d028c8a`  
		Last Modified: Thu, 13 Jul 2023 01:14:16 GMT  
		Size: 145.0 MB (144957090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2f0e46cfe1041dd1036483a699d59215a95b89bcd5ca1b2bb3bbd4d65f1026`  
		Last Modified: Thu, 13 Jul 2023 01:43:30 GMT  
		Size: 16.9 MB (16885038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968d4bb8ef342390cac2f384556f0c86f975b2195be463abd529b84d9ece4a3c`  
		Last Modified: Thu, 13 Jul 2023 01:43:28 GMT  
		Size: 1.6 KB (1613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
