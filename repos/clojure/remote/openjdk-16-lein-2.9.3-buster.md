## `clojure:openjdk-16-lein-2.9.3-buster`

```console
$ docker pull clojure@sha256:a392cc3eed27f616c0f4a2b8afa9045110f5c53afe48bf1192f61f76be83d0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-lein-2.9.3-buster` - linux; amd64

```console
$ docker pull clojure@sha256:0ec6f152b92ab3bd70aaa2ac6425ff0bd6099817efa0fd30b29d67dabcb7ee59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.6 MB (348573538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f411c001bced099b85527bf130398559169337df240bbd16611e4c5c87c15ab1`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:59:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:59:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:58:20 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 06:58:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Thu, 10 Sep 2020 06:58:21 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:58:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 17 Sep 2020 23:31:06 GMT
ENV JAVA_VERSION=16-ea+16
# Thu, 17 Sep 2020 23:31:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/16/GPL/openjdk-16-ea+16_linux-aarch64_bin.tar.gz; 			downloadSha256=6ed6f286820b9989bb460491294379eb0ec7cd689412b22151046d14ffe828be; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/16/GPL/openjdk-16-ea+16_linux-x64_bin.tar.gz; 			downloadSha256=7c57d737cded2e81487401049e9c49d505dbcfe1bc752d5ac0ee1fb8bdc611b3; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Sep 2020 23:31:20 GMT
CMD ["jshell"]
# Fri, 18 Sep 2020 01:27:57 GMT
ENV LEIN_VERSION=2.9.3
# Fri, 18 Sep 2020 01:27:57 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 18 Sep 2020 01:27:57 GMT
WORKDIR /tmp
# Fri, 18 Sep 2020 01:28:04 GMT
RUN apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "42e18e8a833b863ddfba1c5565bd5d78b54bcee661ec86e94a8bdc67b1733e63 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Fri, 18 Sep 2020 01:28:04 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 18 Sep 2020 01:28:05 GMT
ENV LEIN_ROOT=1
# Fri, 18 Sep 2020 01:28:09 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 18 Sep 2020 01:28:09 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e126169501d71bbbd0d3c8d9f35836c41660869fe8432ac606341ed21f7adb`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 7.8 MB (7811567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af28a55c3f320826db8df3146a2c198f9042877ef679f9e32210aa9a7fac9ef`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 10.0 MB (9996317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f1c9932170e54fface2382b2550b8052ae3d41f27e66ea1294e2055dd2b2e7`  
		Last Modified: Thu, 10 Sep 2020 01:15:45 GMT  
		Size: 51.8 MB (51829661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3d7a99945b02edffc7d5f3ab0caf2e3fda405fdca68c63269b9c98a5c6d96c`  
		Last Modified: Thu, 10 Sep 2020 07:08:50 GMT  
		Size: 13.9 MB (13920221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a87cca127971d8c55b4e17c6e458b993591021368f977b189a39e8d2f54feb7`  
		Last Modified: Thu, 10 Sep 2020 07:08:45 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d259e5e82b20852eb0004e2ca26a25894783addd929933b56fc9ffcc2039c71`  
		Last Modified: Thu, 17 Sep 2020 23:35:39 GMT  
		Size: 196.9 MB (196910767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b94ce13e18e1717aab5ff278bc9bb821b96a0c75b36d20dae8bbf4a0b0389f1`  
		Last Modified: Fri, 18 Sep 2020 01:33:14 GMT  
		Size: 13.5 MB (13540689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2c123a7564f2ae39fa2cc7f60366cdd985963e987dd87f4a726f7adcf2357b`  
		Last Modified: Fri, 18 Sep 2020 01:33:14 GMT  
		Size: 4.2 MB (4168192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
