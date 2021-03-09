## `clojure:openjdk-17-lein-slim-buster`

```console
$ docker pull clojure@sha256:66c957a52b309fd11935b9540e6ebcf68d235659883280a2c34147215531d64b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-lein-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:2c404b7dcb6ef0d8e7262a41b6d1b357dbd712c5411fc7cc9ecd26adc455fd96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.5 MB (232456584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e034d8c056190f7fd2f2fddc7e739df8840ac308abe36ca8987b8592ceac777c`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Mar 2021 20:57:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 20:57:00 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 09 Mar 2021 20:57:00 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:57:01 GMT
ENV LANG=C.UTF-8
# Tue, 09 Mar 2021 20:57:01 GMT
ENV JAVA_VERSION=17-ea+12
# Tue, 09 Mar 2021 20:57:14 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/12/GPL/openjdk-17-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='e281f7d1fd2aaa858b02d5be451c51a9ed836c78d002cb82b114e6c36041eebf'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/12/GPL/openjdk-17-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='e2ae713390655d0cfd8302cb2c840553404a3e366162ba5b9a2410ea7b6f1c27'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 20:57:15 GMT
CMD ["jshell"]
# Tue, 09 Mar 2021 21:52:51 GMT
ENV LEIN_VERSION=2.9.5
# Tue, 09 Mar 2021 21:52:51 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 09 Mar 2021 21:52:51 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:53:01 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 09 Mar 2021 21:53:01 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 09 Mar 2021 21:53:01 GMT
ENV LEIN_ROOT=1
# Tue, 09 Mar 2021 21:53:05 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.2"]])' > project.clj   && lein deps && rm project.clj
# Tue, 09 Mar 2021 21:53:05 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f1fbf102b7eaa0998133d35bbcc37641d4d23626a4a2673cb9a2393cb7c34c`  
		Last Modified: Tue, 09 Mar 2021 21:10:48 GMT  
		Size: 3.3 MB (3268548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60033037970287668651b5d2bfc83380fc9a7acf986111f0c596df775670ba8c`  
		Last Modified: Tue, 09 Mar 2021 21:11:03 GMT  
		Size: 186.1 MB (186089454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b3aea075be6b932acdf9bfc3aa6c4eae2e4e27ae11b8c8603c5cf0e6085e64`  
		Last Modified: Tue, 09 Mar 2021 22:08:43 GMT  
		Size: 11.8 MB (11798329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fb643b4158769d503e7323fc96bb9cbd4c2b6257d2dba77125ede5e67f5bea`  
		Last Modified: Tue, 09 Mar 2021 22:08:35 GMT  
		Size: 4.2 MB (4205111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-lein-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b04a10f99e9094023634dcd9344d46995edbb881c89c77028c8f081339df4aa8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.1 MB (227088294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7a382d7c1caa708971e2238c1d278e5075dcb4b6cd499811b80543e85b08b99`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 07:12:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 07:12:09 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 09 Feb 2021 07:12:10 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 07:12:11 GMT
ENV LANG=C.UTF-8
# Thu, 04 Mar 2021 01:12:45 GMT
ENV JAVA_VERSION=17-ea+12
# Thu, 04 Mar 2021 01:13:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/12/GPL/openjdk-17-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='e281f7d1fd2aaa858b02d5be451c51a9ed836c78d002cb82b114e6c36041eebf'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/12/GPL/openjdk-17-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='e2ae713390655d0cfd8302cb2c840553404a3e366162ba5b9a2410ea7b6f1c27'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 04 Mar 2021 01:13:11 GMT
CMD ["jshell"]
# Thu, 04 Mar 2021 01:53:55 GMT
ENV LEIN_VERSION=2.9.5
# Thu, 04 Mar 2021 01:53:56 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 04 Mar 2021 01:53:57 GMT
WORKDIR /tmp
# Thu, 04 Mar 2021 01:54:16 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 04 Mar 2021 01:54:17 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 04 Mar 2021 01:54:18 GMT
ENV LEIN_ROOT=1
# Thu, 04 Mar 2021 01:54:24 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.2"]])' > project.clj   && lein deps && rm project.clj
# Thu, 04 Mar 2021 01:54:25 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96062c0c15f683e4abb09efb938dfd7ff23002f72a375c75492d44bde3a6c26f`  
		Last Modified: Tue, 09 Feb 2021 07:22:32 GMT  
		Size: 3.1 MB (3118711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc7dd6381fbbe8b834b16e6b9e05a717a47650bce0d9dc82dcb5b6a23e14d1c`  
		Last Modified: Thu, 04 Mar 2021 01:19:03 GMT  
		Size: 182.1 MB (182114603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a74440c0c108d7ff28f29013f2421b176e9b5ea01d14b055988e581b64ef8e0`  
		Last Modified: Thu, 04 Mar 2021 02:00:02 GMT  
		Size: 11.8 MB (11798405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc24efb71f0ae93f371693521adc5712738f7058e39b3eebca5c5b7adbc6502e`  
		Last Modified: Thu, 04 Mar 2021 02:00:01 GMT  
		Size: 4.2 MB (4205126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
