## `clojure:openjdk-18-lein`

```console
$ docker pull clojure@sha256:53ad5060d20ade811f3695a348590c9f7abe38da5b2f10254472efe2e66a5476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-lein` - linux; amd64

```console
$ docker pull clojure@sha256:7d1c8388b415122d46fefa2a867c06c760ca8971f792b5a7f5287af468d4f7a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234319420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:655abfeb988138b07d19a5b25be72aca13611387ebd6499566504aa04fe961d4`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:53:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 17 Aug 2021 06:53:11 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:53:11 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 17:32:05 GMT
ENV JAVA_VERSION=18-ea+12
# Fri, 27 Aug 2021 17:32:18 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/12/GPL/openjdk-18-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='a9bc316abb2e03378f35fc574685b8bbdd15cd6803df70c02e71ff8f19ad292b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/12/GPL/openjdk-18-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='08129b3c4ef9956a14a7112565a185ac9ea7e3b327875089114ce6fe2563f585'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 27 Aug 2021 17:32:19 GMT
CMD ["jshell"]
# Sat, 28 Aug 2021 01:23:46 GMT
ENV LEIN_VERSION=2.9.6
# Sat, 28 Aug 2021 01:23:47 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sat, 28 Aug 2021 01:23:47 GMT
WORKDIR /tmp
# Sat, 28 Aug 2021 01:23:59 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Sat, 28 Aug 2021 01:23:59 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 28 Aug 2021 01:24:00 GMT
ENV LEIN_ROOT=1
# Sat, 28 Aug 2021 01:24:04 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Sat, 28 Aug 2021 01:24:05 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4da59afefd4321f8d175c5bd1b393c479d6733a58eece9df143ca37c633fd7`  
		Last Modified: Fri, 27 Aug 2021 17:42:30 GMT  
		Size: 187.9 MB (187897894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a50e40231e07519e1c67ede0fd5933a57001f3a26fc82a3548804a28e7cff78`  
		Last Modified: Sat, 28 Aug 2021 01:29:22 GMT  
		Size: 11.8 MB (11803052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf04f8f0ec5d105264200d7b9273d55651cd7e8166a9af13b31e5079f9dc76a`  
		Last Modified: Sat, 28 Aug 2021 01:29:22 GMT  
		Size: 4.2 MB (4203721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-lein` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:dc38edb27052a0f9491ef47560d51c5d9a07a3b03dfd548436bb18ebcffc85c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231673649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:889df4ec9cf1cd0f0710f5b58fbb4bc86722f64921136696ef5c2bbb3cfb3528`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:04:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:04:05 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 17 Aug 2021 06:04:06 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:04:06 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 17:51:00 GMT
ENV JAVA_VERSION=18-ea+12
# Fri, 27 Aug 2021 17:51:17 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/12/GPL/openjdk-18-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='a9bc316abb2e03378f35fc574685b8bbdd15cd6803df70c02e71ff8f19ad292b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/12/GPL/openjdk-18-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='08129b3c4ef9956a14a7112565a185ac9ea7e3b327875089114ce6fe2563f585'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 27 Aug 2021 17:51:18 GMT
CMD ["jshell"]
# Sat, 28 Aug 2021 01:58:18 GMT
ENV LEIN_VERSION=2.9.6
# Sat, 28 Aug 2021 01:58:18 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sat, 28 Aug 2021 01:58:18 GMT
WORKDIR /tmp
# Sat, 28 Aug 2021 01:58:35 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Sat, 28 Aug 2021 01:58:35 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 28 Aug 2021 01:58:35 GMT
ENV LEIN_ROOT=1
# Sat, 28 Aug 2021 01:58:38 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Sat, 28 Aug 2021 01:58:38 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82a27af984eefbe6b82ccb775aead56e92f82cf16d079218087ebe132125cf5`  
		Last Modified: Tue, 17 Aug 2021 06:15:41 GMT  
		Size: 3.1 MB (3118861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c2f7b6d0e50c72cec02e8f9f1af7f75a17bdd36f40add0a16696f37c596a71`  
		Last Modified: Fri, 27 Aug 2021 18:07:39 GMT  
		Size: 186.6 MB (186633190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2202fd25585475b82a316bbd886c24d81df83c59512b05088f3ee065092b91`  
		Last Modified: Sat, 28 Aug 2021 02:10:25 GMT  
		Size: 11.8 MB (11802847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85eaffcdcf2bdd11bfc1bb40c259a3fe16a1c1accd45e85a97943b1524674a2`  
		Last Modified: Sat, 28 Aug 2021 02:10:25 GMT  
		Size: 4.2 MB (4203679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
