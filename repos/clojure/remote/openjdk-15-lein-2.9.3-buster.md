## `clojure:openjdk-15-lein-2.9.3-buster`

```console
$ docker pull clojure@sha256:0f2442b408a3e8c39515068c0e3656a13e207a64816d0c8b440ce543e2095cd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-15-lein-2.9.3-buster` - linux; amd64

```console
$ docker pull clojure@sha256:4a200a7263b5f3a807fc224a0c62189deeb6c43c5f1608959224f8533ebb68f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.5 MB (347523923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e38d3c29eca19df6bb46993bcb54eb9fc17165cacb4124d2c5df38ab3e87003e`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:30 GMT
ADD file:6627ad39ea0cb9fcb212342326d14efaff51aece1fd0dc16d5bbcaa25d858622 in / 
# Tue, 13 Oct 2020 01:38:30 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:14:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:14:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 02:15:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:57:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:57:38 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 08:59:34 GMT
ENV JAVA_HOME=/usr/local/openjdk-15
# Tue, 13 Oct 2020 08:59:34 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 08:59:35 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 13 Oct 2020 08:59:35 GMT
ENV JAVA_VERSION=15
# Tue, 13 Oct 2020 09:00:14 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-aarch64_bin.tar.gz; 			downloadSha256=01e7e07dd8a67a65b32fdcaff75ba3f21cd9cfc749287e7c9b1c6037f96a3537; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-x64_bin.tar.gz; 			downloadSha256=bb67cadee687d7b486583d03c9850342afea4593be4f436044d785fba9508fb7; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Oct 2020 09:00:15 GMT
CMD ["jshell"]
# Wed, 14 Oct 2020 05:35:29 GMT
ENV LEIN_VERSION=2.9.3
# Wed, 14 Oct 2020 05:35:29 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 14 Oct 2020 05:35:29 GMT
WORKDIR /tmp
# Wed, 14 Oct 2020 05:35:35 GMT
RUN apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "42e18e8a833b863ddfba1c5565bd5d78b54bcee661ec86e94a8bdc67b1733e63 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Wed, 14 Oct 2020 05:35:35 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 14 Oct 2020 05:35:35 GMT
ENV LEIN_ROOT=1
# Wed, 14 Oct 2020 05:35:40 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 14 Oct 2020 05:35:40 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:e4c3d3e4f7b024979a1c12daa4073f6353b2ba92d96418bc90451994927c9bff`  
		Last Modified: Tue, 13 Oct 2020 01:48:02 GMT  
		Size: 50.4 MB (50395978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101c41d0463bc77661fb3343235b16d536a92d2efb687046164d413e51bd4fc4`  
		Last Modified: Tue, 13 Oct 2020 02:28:35 GMT  
		Size: 7.8 MB (7811737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8275efcd805f9905d7def23603618236284b0be6b9e47455c638fbfb03fa9208`  
		Last Modified: Tue, 13 Oct 2020 02:28:35 GMT  
		Size: 10.0 MB (9996326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751620502a7a2905067c2f32d4982fb9b310b9808670ce82c0e2b40f5307a3ee`  
		Last Modified: Tue, 13 Oct 2020 02:28:53 GMT  
		Size: 51.8 MB (51829492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f28f646e98144707f2cc19e3ad498b86228306ce9f907e555f8f055d690dd1`  
		Last Modified: Tue, 13 Oct 2020 09:07:43 GMT  
		Size: 13.9 MB (13920357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e4347bd28dba027922cc9f428d224f8abdadad4d530b6116dc9b1405e39ea7`  
		Last Modified: Tue, 13 Oct 2020 09:08:40 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f409e07f070218b88694c503cc3e058043e183b63ad5e460b3d4bc0a93111ba2`  
		Last Modified: Tue, 13 Oct 2020 09:08:59 GMT  
		Size: 195.9 MB (195861032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e7630828c8b927e3e9122bd0a9712037f3eb6996246274c7b60c976b227f7e`  
		Last Modified: Wed, 14 Oct 2020 05:45:32 GMT  
		Size: 13.5 MB (13540650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3245c731a96639f53317ecf338c9998bde83f554978211237c96c2337781b40`  
		Last Modified: Wed, 14 Oct 2020 05:45:32 GMT  
		Size: 4.2 MB (4168142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
