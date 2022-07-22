## `jetty:9-jdk8-alpine-amazoncorretto`

```console
$ docker pull jetty@sha256:a656df7ffec8f01eff89200f01e0c690ba825dcda9024f3a9c968b8a4aac3212
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9-jdk8-alpine-amazoncorretto` - linux; amd64

```console
$ docker pull jetty@sha256:3502abe94030bde8026ee37dfa2193225b6d810e65209f221a9ca9dc01a5e3cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118868477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61b9ca03740620e546bb9c04efb8cb9e42324751af1c67c2c53c7c857fa0fe31`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Fri, 22 Jul 2022 18:20:26 GMT
ARG version=8.342.07.3
# Fri, 22 Jul 2022 18:20:30 GMT
# ARGS: version=8.342.07.3
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Fri, 22 Jul 2022 18:20:30 GMT
ENV LANG=C.UTF-8
# Fri, 22 Jul 2022 18:20:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 22 Jul 2022 18:20:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
# Fri, 22 Jul 2022 19:05:56 GMT
ENV JETTY_VERSION=9.4.48.v20220622
# Fri, 22 Jul 2022 19:05:57 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 22 Jul 2022 19:05:57 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 22 Jul 2022 19:05:57 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 22 Jul 2022 19:05:57 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
# Fri, 22 Jul 2022 19:05:57 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.48.v20220622/jetty-home-9.4.48.v20220622.tar.gz
# Fri, 22 Jul 2022 19:05:57 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 22 Jul 2022 19:06:07 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ; 	apk add --no-cache gnupg curl ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	addgroup -S jetty && adduser -h $JETTY_BASE -S jetty -G jetty; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 22 Jul 2022 19:06:08 GMT
WORKDIR /var/lib/jetty
# Fri, 22 Jul 2022 19:06:08 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Fri, 22 Jul 2022 19:06:08 GMT
USER jetty
# Fri, 22 Jul 2022 19:06:08 GMT
EXPOSE 8080
# Fri, 22 Jul 2022 19:06:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Jul 2022 19:06:08 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd5a4f6ce47945ae64d5a04190fa46841466feaea608b4ae91bd9b8562b09b`  
		Last Modified: Fri, 22 Jul 2022 18:24:24 GMT  
		Size: 98.8 MB (98798057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd4f8b35eb3399eab4c88a10e3b8dd45968abcace3f3de781d7560d98792719`  
		Last Modified: Fri, 22 Jul 2022 19:10:54 GMT  
		Size: 17.3 MB (17254335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6094a00bf1260d9661e041a790b8be6d66699047e3b1d10b48f0650e0a86d064`  
		Last Modified: Fri, 22 Jul 2022 19:10:52 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
