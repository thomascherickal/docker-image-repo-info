## `jetty:10-jdk17-amazoncorretto`

```console
$ docker pull jetty@sha256:8e42cfb0511d5dc966686df9d85e94ee005c7cb8e8a51d34c11556eef12add85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:10-jdk17-amazoncorretto` - linux; amd64

```console
$ docker pull jetty@sha256:c1c85a19d9a23dbd8497283e0f2ecdd6ff8ec5ca39551b7713b192ba048a42ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.3 MB (231324078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f85c1c29a6553183fa25e12239f5740ea301a6457cb7a7e9bbb5b1dd6405f083`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 13 Jul 2023 01:20:13 GMT
COPY dir:be29c71398840090bec7021ae8f2d354451564507602cf38257ad90a915b1838 in / 
# Thu, 13 Jul 2023 01:20:13 GMT
CMD ["/bin/bash"]
# Thu, 13 Jul 2023 01:43:04 GMT
ARG version=17.0.7.7-1
# Thu, 13 Jul 2023 01:43:30 GMT
# ARGS: version=17.0.7.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 13 Jul 2023 01:43:30 GMT
ENV LANG=C.UTF-8
# Thu, 13 Jul 2023 01:43:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Thu, 13 Jul 2023 02:37:38 GMT
ENV JETTY_VERSION=10.0.15
# Thu, 13 Jul 2023 02:37:38 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 13 Jul 2023 02:37:38 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 13 Jul 2023 02:37:38 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 13 Jul 2023 02:37:38 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Jul 2023 02:37:38 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.15/jetty-home-10.0.15.tar.gz
# Thu, 13 Jul 2023 02:37:38 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Thu, 13 Jul 2023 02:37:57 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 13 Jul 2023 02:37:57 GMT
WORKDIR /var/lib/jetty
# Thu, 13 Jul 2023 02:37:57 GMT
COPY multi:88ca540b9901ef22d614e919524f1d550a54166ea9880b0aa9695f8e0470c8f7 in / 
# Thu, 13 Jul 2023 02:37:57 GMT
USER jetty
# Thu, 13 Jul 2023 02:37:57 GMT
EXPOSE 8080
# Thu, 13 Jul 2023 02:37:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 13 Jul 2023 02:37:57 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e90aa42bc48ff728ab10fd485b42144e863dfd8689dd6ea94c78ac0357ec5101`  
		Last Modified: Fri, 30 Jun 2023 00:09:38 GMT  
		Size: 62.5 MB (62485766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bcac5079dea2a4f965ef5cb9f72843b2c88941a2c7582794ba2f7a007540f4`  
		Last Modified: Thu, 13 Jul 2023 01:53:12 GMT  
		Size: 152.0 MB (151984828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788ca73835e503878abdfc385ea7e30246ef6e834ea178058c642fe155d53c67`  
		Last Modified: Thu, 13 Jul 2023 02:42:29 GMT  
		Size: 16.9 MB (16851871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4275345f25d7d7aa2a8dca24a8ffcf285e4f46557005e1e0ae59d1b838e592d3`  
		Last Modified: Thu, 13 Jul 2023 02:42:27 GMT  
		Size: 1.6 KB (1613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:10-jdk17-amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:17bb9755a2e8953a6fa28a3b0cb1175314996a551fc2195dea6c1f5c8ba54725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231504487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8855b1f1bcdf17391e2287d19535f8e592f69afa0d9ec9442e65f3fc60c27d4f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 13 Jul 2023 00:40:00 GMT
COPY dir:a284fdf4a484ebc9131c665fc151094ec73265d07d353476272944e301722064 in / 
# Thu, 13 Jul 2023 00:40:01 GMT
CMD ["/bin/bash"]
# Thu, 13 Jul 2023 01:08:15 GMT
ARG version=17.0.7.7-1
# Thu, 13 Jul 2023 01:08:34 GMT
# ARGS: version=17.0.7.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 13 Jul 2023 01:08:35 GMT
ENV LANG=C.UTF-8
# Thu, 13 Jul 2023 01:08:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Thu, 13 Jul 2023 01:39:47 GMT
ENV JETTY_VERSION=10.0.15
# Thu, 13 Jul 2023 01:39:47 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 13 Jul 2023 01:39:47 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 13 Jul 2023 01:39:47 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 13 Jul 2023 01:39:47 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Jul 2023 01:39:47 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.15/jetty-home-10.0.15.tar.gz
# Thu, 13 Jul 2023 01:39:47 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Thu, 13 Jul 2023 01:40:02 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 13 Jul 2023 01:40:02 GMT
WORKDIR /var/lib/jetty
# Thu, 13 Jul 2023 01:40:02 GMT
COPY multi:88ca540b9901ef22d614e919524f1d550a54166ea9880b0aa9695f8e0470c8f7 in / 
# Thu, 13 Jul 2023 01:40:02 GMT
USER jetty
# Thu, 13 Jul 2023 01:40:02 GMT
EXPOSE 8080
# Thu, 13 Jul 2023 01:40:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 13 Jul 2023 01:40:03 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:20c8bca6ae5daad56b485a4b6f1f395a51727d69eb6a7566c53b00a366e46576`  
		Last Modified: Fri, 30 Jun 2023 17:38:06 GMT  
		Size: 64.1 MB (64128925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f8ad53a63d267a406d699e19a00487a51be1c91f12e3fbfe6fccc716f6ebac`  
		Last Modified: Thu, 13 Jul 2023 01:16:15 GMT  
		Size: 150.5 MB (150487437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c872e1c931e1e25cb729ae8b0a8bbec20465224f68c452c41edec70eb163a5`  
		Last Modified: Thu, 13 Jul 2023 01:43:11 GMT  
		Size: 16.9 MB (16886512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b65202b2e06325748cb9d3ed8b0c0011d41fbc9dcebb1abe7580f78f551c1d8`  
		Last Modified: Thu, 13 Jul 2023 01:43:10 GMT  
		Size: 1.6 KB (1613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
