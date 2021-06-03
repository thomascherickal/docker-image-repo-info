## `jetty:latest`

```console
$ docker pull jetty@sha256:422a768c9d1b773189fc0a9cc50cec3331c0d03567511fa20f2e738b3a0a18a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:latest` - linux; amd64

```console
$ docker pull jetty@sha256:5da38cd5281f26bec5af9692839237af6bbb646b16ae87e5a76f6f5a766abc90
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250206460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37ef30ec3302089f31aecb82953a9f330744547816f8f55b52c20e9210771c0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Wed, 02 Jun 2021 17:21:00 GMT
ADD file:b4c18f27ab03ed63f96174673a8d97d4b1b6abb552b6fe3201c6aec934e8312f in / 
# Wed, 02 Jun 2021 17:21:00 GMT
CMD ["/bin/bash"]
# Wed, 02 Jun 2021 17:37:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 02 Jun 2021 17:38:32 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Wed, 02 Jun 2021 17:38:33 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 17:38:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Jun 2021 17:38:33 GMT
ENV JAVA_VERSION=16.0.1
# Wed, 02 Jun 2021 17:38:46 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='b1198ffffb7d26a3fdedc0fa599f60a0d12aa60da1714b56c1defbce95d8b235'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='602b005074777df2a0b4306e20152a6446803edd87ccbab95b2f313c4d9be6ba'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 02 Jun 2021 17:38:47 GMT
CMD ["jshell"]
# Wed, 02 Jun 2021 18:07:15 GMT
ENV JETTY_VERSION=9.4.41.v20210516
# Wed, 02 Jun 2021 18:07:15 GMT
ENV JETTY_HOME=/usr/local/jetty
# Wed, 02 Jun 2021 18:07:15 GMT
ENV JETTY_BASE=/var/lib/jetty
# Wed, 02 Jun 2021 18:07:15 GMT
ENV TMPDIR=/tmp/jetty
# Wed, 02 Jun 2021 18:07:15 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 18:07:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.41.v20210516/jetty-home-9.4.41.v20210516.tar.gz
# Wed, 02 Jun 2021 18:07:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Wed, 02 Jun 2021 18:07:19 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			p80.pool.sks-keyservers.net:80 			ipv4.pool.sks-keyservers.net 			pgp.mit.edu ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Wed, 02 Jun 2021 18:07:19 GMT
WORKDIR /var/lib/jetty
# Wed, 02 Jun 2021 18:07:20 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Wed, 02 Jun 2021 18:07:20 GMT
USER jetty
# Wed, 02 Jun 2021 18:07:20 GMT
EXPOSE 8080
# Wed, 02 Jun 2021 18:07:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 18:07:20 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:5a581c13a8b96af42c06955acd88fdb3aff53edcbdd33faa7bca9854fd8bfbaf`  
		Last Modified: Wed, 02 Jun 2021 17:22:10 GMT  
		Size: 42.2 MB (42183647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cd02acd9c2b40dba18c3fe68882bcb5ebda0caeb5e550965d9ac81e3b55fbf`  
		Last Modified: Wed, 02 Jun 2021 17:43:15 GMT  
		Size: 13.4 MB (13400021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66727af51578917387f3fdc9ad6ed2d9fe890d4ad0f4523afc868b58b2e832e1`  
		Last Modified: Wed, 02 Jun 2021 17:44:35 GMT  
		Size: 184.8 MB (184799527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e84cda7653f7db6d8d9a8fd5660d357c6c9658fa3f73f86ff9ac2a92e4c952d`  
		Last Modified: Wed, 02 Jun 2021 18:09:13 GMT  
		Size: 9.8 MB (9821818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252c28ff5c0c7053e5473b9b3a7cc7b5991c93f9c1e55c80d99516058172a830`  
		Last Modified: Wed, 02 Jun 2021 18:09:12 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
