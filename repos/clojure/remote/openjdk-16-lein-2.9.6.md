## `clojure:openjdk-16-lein-2.9.6`

```console
$ docker pull clojure@sha256:3691fb94e2e1a566abba48807da59d6f4618212358aef0dc657244da53835b38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-16-lein-2.9.6` - linux; amd64

```console
$ docker pull clojure@sha256:c0465ddb0d82f1829fcf8e9a789be3c68270f256cf87dc0a385382d4aa2a2e7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231597345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65ec381c9283680e16492ba3131ce775bf28eca02edf1ae4526fe00f01691304`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:00:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:02:29 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Wed, 23 Jun 2021 08:02:29 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 08:02:29 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 08:02:29 GMT
ENV JAVA_VERSION=16.0.1
# Wed, 23 Jun 2021 08:02:46 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='b1198ffffb7d26a3fdedc0fa599f60a0d12aa60da1714b56c1defbce95d8b235'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='602b005074777df2a0b4306e20152a6446803edd87ccbab95b2f313c4d9be6ba'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 23 Jun 2021 08:02:47 GMT
CMD ["jshell"]
# Thu, 24 Jun 2021 02:42:51 GMT
ENV LEIN_VERSION=2.9.6
# Thu, 24 Jun 2021 02:42:51 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 24 Jun 2021 02:42:51 GMT
WORKDIR /tmp
# Thu, 24 Jun 2021 02:43:02 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 24 Jun 2021 02:43:02 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 24 Jun 2021 02:43:02 GMT
ENV LEIN_ROOT=1
# Thu, 24 Jun 2021 02:43:06 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Thu, 24 Jun 2021 02:43:06 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee45ae9730633057cf9bd12924f9a1bf2b590631d3d085b14c96f4466557794`  
		Last Modified: Wed, 23 Jun 2021 08:12:04 GMT  
		Size: 3.3 MB (3268886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd24cb1363715cab6b066cccbcdfb412215d244ff8cf0038145d0246f6ca10c`  
		Last Modified: Wed, 23 Jun 2021 08:16:21 GMT  
		Size: 185.2 MB (185175871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b0331455d8280a43ed983b20728443257c00c83003ead9e1ad8f84b6756dc7`  
		Last Modified: Thu, 24 Jun 2021 02:53:39 GMT  
		Size: 11.8 MB (11803046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c667644b06db1cb0b0f02798d4e1cfcae060791510fff3fecf342e36942a2d`  
		Last Modified: Thu, 24 Jun 2021 02:53:38 GMT  
		Size: 4.2 MB (4203691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-16-lein-2.9.6` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b737550af6e212daacb9c1197128bcbf85da6eaddb494d715f698e86e1f4d43e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.6 MB (224598809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dcb3a9e83c3117f200c8293f28f38cfe3625c3a2f1ac8575972fcc93466318b`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 04:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 04:58:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Wed, 23 Jun 2021 04:58:21 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 04:58:21 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 04:58:21 GMT
ENV JAVA_VERSION=16.0.1
# Wed, 23 Jun 2021 04:58:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='b1198ffffb7d26a3fdedc0fa599f60a0d12aa60da1714b56c1defbce95d8b235'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='602b005074777df2a0b4306e20152a6446803edd87ccbab95b2f313c4d9be6ba'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 23 Jun 2021 04:58:34 GMT
CMD ["jshell"]
# Wed, 23 Jun 2021 19:58:07 GMT
ENV LEIN_VERSION=2.9.6
# Wed, 23 Jun 2021 19:58:07 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 23 Jun 2021 19:58:08 GMT
WORKDIR /tmp
# Wed, 23 Jun 2021 19:58:17 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 23 Jun 2021 19:58:17 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 23 Jun 2021 19:58:17 GMT
ENV LEIN_ROOT=1
# Wed, 23 Jun 2021 19:58:21 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Wed, 23 Jun 2021 19:58:21 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb5c013aa648ff2c30dafc35db9efb2faa7f9fa6f1c98a2f31c1b5fee0334dc`  
		Last Modified: Wed, 23 Jun 2021 05:11:10 GMT  
		Size: 3.1 MB (3118894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f933fcbcc981b073247ef4de4fa9f95dbfe58a932631b03dae69d8025f465e52`  
		Last Modified: Wed, 23 Jun 2021 05:15:44 GMT  
		Size: 179.6 MB (179558374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deea531e9ca65747a3232a95f04e94f6c992af4e88c6ff001270f3a82a927e9b`  
		Last Modified: Wed, 23 Jun 2021 20:09:23 GMT  
		Size: 11.8 MB (11802866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fcd7ce300829e629726b741d5022d95691c7a4e420757f6e55bc21f6d19f36f`  
		Last Modified: Wed, 23 Jun 2021 20:09:22 GMT  
		Size: 4.2 MB (4203682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
