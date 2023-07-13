## `jetty:9-amazoncorretto`

```console
$ docker pull jetty@sha256:42fb6b3cb58a0958946e2e8724ec994a190dbda2a31db81c7dfe843f1a16f42c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9-amazoncorretto` - linux; amd64

```console
$ docker pull jetty@sha256:795deac6ac3f1c4422b954fc2ac03d605cac4c03ca89dcf830323140d75f0768
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.3 MB (230281160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4e16ef6c10b2ab4ead6ad456d59b384e019e39f1fccfb580c7a992ee48eb6ba`
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
# Thu, 13 Jul 2023 02:35:52 GMT
ENV JETTY_VERSION=9.4.51.v20230217
# Thu, 13 Jul 2023 02:35:52 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 13 Jul 2023 02:35:52 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 13 Jul 2023 02:35:52 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 13 Jul 2023 02:35:52 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Jul 2023 02:35:52 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.51.v20230217/jetty-home-9.4.51.v20230217.tar.gz
# Thu, 13 Jul 2023 02:35:52 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Thu, 13 Jul 2023 02:36:11 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 13 Jul 2023 02:36:11 GMT
WORKDIR /var/lib/jetty
# Thu, 13 Jul 2023 02:36:11 GMT
COPY multi:88ca540b9901ef22d614e919524f1d550a54166ea9880b0aa9695f8e0470c8f7 in / 
# Thu, 13 Jul 2023 02:36:11 GMT
USER jetty
# Thu, 13 Jul 2023 02:36:11 GMT
EXPOSE 8080
# Thu, 13 Jul 2023 02:36:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 13 Jul 2023 02:36:12 GMT
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
	-	`sha256:d0d4256413d6bdb5e1aa516cf3be2f1db258a7fb4e233eb68ba80bc6e37ba0c7`  
		Last Modified: Thu, 13 Jul 2023 02:41:25 GMT  
		Size: 15.8 MB (15808953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83fe021bb388dd1e48530cff93109ecf379770e5544454d0c6ce2eb8cde3c6f`  
		Last Modified: Thu, 13 Jul 2023 02:41:24 GMT  
		Size: 1.6 KB (1613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9-amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:ccad39d1fe1ad984332c357058f29988f62bdc916d9c03c5cfb264b2ed09d651
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230458063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8f80b18cc5df19ba90c2c0c1ce43fa1a3d5489b53ed00d0b97cbcec2ddd35b`
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
# Thu, 13 Jul 2023 01:38:29 GMT
ENV JETTY_VERSION=9.4.51.v20230217
# Thu, 13 Jul 2023 01:38:30 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 13 Jul 2023 01:38:30 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 13 Jul 2023 01:38:30 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 13 Jul 2023 01:38:30 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Jul 2023 01:38:30 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.51.v20230217/jetty-home-9.4.51.v20230217.tar.gz
# Thu, 13 Jul 2023 01:38:30 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Thu, 13 Jul 2023 01:38:45 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ;     yum install -y shadow-utils tar xz gzip && yum clean all ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 13 Jul 2023 01:38:45 GMT
WORKDIR /var/lib/jetty
# Thu, 13 Jul 2023 01:38:46 GMT
COPY multi:88ca540b9901ef22d614e919524f1d550a54166ea9880b0aa9695f8e0470c8f7 in / 
# Thu, 13 Jul 2023 01:38:46 GMT
USER jetty
# Thu, 13 Jul 2023 01:38:46 GMT
EXPOSE 8080
# Thu, 13 Jul 2023 01:38:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 13 Jul 2023 01:38:46 GMT
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
	-	`sha256:fc3e8af91d7fd5ac0157688f8835f129560283cdbd3923363b3ffa4ee1f55627`  
		Last Modified: Thu, 13 Jul 2023 01:42:11 GMT  
		Size: 15.8 MB (15840088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba063c887d31ead53df5a31320f165958ca978a2be5e9aff1d2e88a2fde3bc`  
		Last Modified: Thu, 13 Jul 2023 01:42:10 GMT  
		Size: 1.6 KB (1613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
