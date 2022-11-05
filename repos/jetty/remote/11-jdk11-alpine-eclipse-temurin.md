## `jetty:11-jdk11-alpine-eclipse-temurin`

```console
$ docker pull jetty@sha256:3c745a7f799aa490d37f58da9d51c9f5686825afc43e1df7a2a00e08592e592c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:11-jdk11-alpine-eclipse-temurin` - linux; amd64

```console
$ docker pull jetty@sha256:6db73166dfa8984f8dab91776b86a4e3eae2e91ea3e153b270912f26557869a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.3 MB (230330619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40020e4ccaa0269abc022e4b1feb1701647fafdd4c828aef137d243fe7e3e428`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 16:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 07 Oct 2022 16:53:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 16:53:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Oct 2022 16:53:21 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Fri, 04 Nov 2022 23:20:57 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:21:21 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='774d5955c09893dda14e3eb0fd3e239a6b2cec58615fcf4ec68747260b6e1cc1';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Fri, 04 Nov 2022 23:21:24 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:21:24 GMT
CMD ["jshell"]
# Sat, 05 Nov 2022 00:16:16 GMT
ENV JETTY_VERSION=11.0.12
# Sat, 05 Nov 2022 00:16:16 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 05 Nov 2022 00:16:16 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 05 Nov 2022 00:16:16 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 05 Nov 2022 00:16:17 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 00:16:17 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/11.0.12/jetty-home-11.0.12.tar.gz
# Sat, 05 Nov 2022 00:16:17 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Sat, 05 Nov 2022 00:16:27 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ; 	apk add --no-cache gnupg curl ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	addgroup -S jetty && adduser -h $JETTY_BASE -S jetty -G jetty; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 05 Nov 2022 00:16:27 GMT
WORKDIR /var/lib/jetty
# Sat, 05 Nov 2022 00:16:27 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Sat, 05 Nov 2022 00:16:27 GMT
USER jetty
# Sat, 05 Nov 2022 00:16:28 GMT
EXPOSE 8080
# Sat, 05 Nov 2022 00:16:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 05 Nov 2022 00:16:28 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5835cc7e6eb64b728c9694dd72d8aede877af0a2ec44f981847853af9abbf5`  
		Last Modified: Fri, 07 Oct 2022 16:57:51 GMT  
		Size: 12.0 MB (12041341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326222305ee7ba2cd4c5b9421222ea3b98c1fcdf5614f10686612cd9e48d4944`  
		Last Modified: Fri, 04 Nov 2022 23:27:19 GMT  
		Size: 193.8 MB (193812570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f17b778e5911ba3c3e61d32e7eeb30f4b62bf95d1ced95b7cf7c1f152fe40da`  
		Last Modified: Fri, 04 Nov 2022 23:27:05 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfda8b2ad83b085ec2366f9b7ca02774457042bff6aaffa80559805006df88c5`  
		Last Modified: Sat, 05 Nov 2022 00:25:49 GMT  
		Size: 21.7 MB (21669033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dc08b88589e694dbe810a7421204629da29505210e4652fb7bf509a62d4a07`  
		Last Modified: Sat, 05 Nov 2022 00:25:47 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
