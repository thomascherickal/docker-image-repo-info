## `clojure:openjdk-17-slim-buster`

```console
$ docker pull clojure@sha256:15f0f802cf5907fe81c243abb9ccc08c3e102c1d2c77d49669ac90d6f2c8a5ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:a9f7010d5bf99d674713f3185def513e044e0f646070f8cec89b7b38144f6a71
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (233967730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a441a31eefe37aa10172ed91088da8ff7115fd409b0b5fb5eec712360041aef2`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:00:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:01:12 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 23 Jun 2021 08:01:12 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 08:01:12 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 08:01:12 GMT
ENV JAVA_VERSION=17-ea+27
# Wed, 23 Jun 2021 08:01:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/27/GPL/openjdk-17-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='7e1042e3daf741aad75ebda0ea38650111475a810be8fedf38f554732d7750f4'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/27/GPL/openjdk-17-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='88bdeb49442e85c19e126b720bd810bc59007973c6fc06aa6e62b609c1c44d53'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 23 Jun 2021 08:01:30 GMT
CMD ["jshell"]
# Thu, 24 Jun 2021 02:44:59 GMT
ENV LEIN_VERSION=2.9.6
# Thu, 24 Jun 2021 02:44:59 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 24 Jun 2021 02:44:59 GMT
WORKDIR /tmp
# Thu, 24 Jun 2021 02:45:09 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 24 Jun 2021 02:45:09 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 24 Jun 2021 02:45:09 GMT
ENV LEIN_ROOT=1
# Thu, 24 Jun 2021 02:45:13 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Thu, 24 Jun 2021 02:45:14 GMT
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
	-	`sha256:aded171439b9acb04d47c919182bd77c6d2365bf28cf402ee2db0e3821f7342b`  
		Last Modified: Wed, 23 Jun 2021 08:14:13 GMT  
		Size: 187.5 MB (187546175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385ae38db811799194d3ebc14e7bc550d8726020e5203a8186dfdc9c66a92652`  
		Last Modified: Thu, 24 Jun 2021 02:55:23 GMT  
		Size: 11.8 MB (11803096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad9a79432d1ef1f746b81468afbcba5797fc03221a0983b65b5b51e704aff26`  
		Last Modified: Thu, 24 Jun 2021 02:55:22 GMT  
		Size: 4.2 MB (4203722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:96fcee5d301d120575ecf0acae4f5019be8b298bd3c263e4f033b05bab88d436
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.4 MB (231398027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e84ab32fbbeb87401a42f8b4233a7c0f87a9684ac867a94f1aa0b3c448111a`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 04:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 04:57:10 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 23 Jun 2021 04:57:10 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 04:57:10 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 04:57:10 GMT
ENV JAVA_VERSION=17-ea+27
# Wed, 23 Jun 2021 04:57:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/27/GPL/openjdk-17-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='7e1042e3daf741aad75ebda0ea38650111475a810be8fedf38f554732d7750f4'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/27/GPL/openjdk-17-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='88bdeb49442e85c19e126b720bd810bc59007973c6fc06aa6e62b609c1c44d53'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 23 Jun 2021 04:57:23 GMT
CMD ["jshell"]
# Wed, 23 Jun 2021 20:00:30 GMT
ENV LEIN_VERSION=2.9.6
# Wed, 23 Jun 2021 20:00:30 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 23 Jun 2021 20:00:30 GMT
WORKDIR /tmp
# Wed, 23 Jun 2021 20:00:45 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 23 Jun 2021 20:00:46 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 23 Jun 2021 20:00:46 GMT
ENV LEIN_ROOT=1
# Wed, 23 Jun 2021 20:00:49 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Wed, 23 Jun 2021 20:00:49 GMT
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
	-	`sha256:94cc1fe036d48b434be9ff64dcce132db5120a6f2c84577f627ca47e01e62879`  
		Last Modified: Wed, 23 Jun 2021 05:13:28 GMT  
		Size: 186.4 MB (186357568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c2179f72664b48b660ed3b5c1f6b42e147ee285438eefbecc434d305986feb`  
		Last Modified: Wed, 23 Jun 2021 20:11:30 GMT  
		Size: 11.8 MB (11802848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259e67bb59356dfd3188404a692e07b95f74679f064c64523e4730c60ed31740`  
		Last Modified: Wed, 23 Jun 2021 20:11:29 GMT  
		Size: 4.2 MB (4203724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
