## `clojure:openjdk-14-lein-2.9.1`

```console
$ docker pull clojure@sha256:37741d75d7e4087d0139a912d11da8d39e760850ec34f19367033f4ec83c4776
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-14-lein-2.9.1` - linux; amd64

```console
$ docker pull clojure@sha256:100a938700c5cc6b5ee0b607e6ce4c4512d89deef52e86dd64f96a5cfbee5838
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.7 MB (251737787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e47806e624478a6885633133d3b1fae3def1e0d0b16737081d893f0dd2b5db9`
-	Default Command: `["lein","repl"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:22:53 GMT
ENV JAVA_HOME=/usr/java/openjdk-14
# Sun, 02 Feb 2020 06:22:53 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:22:55 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:22:55 GMT
ENV JAVA_VERSION=14-ea+34
# Sun, 02 Feb 2020 06:22:56 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk14/34/GPL/openjdk-14-ea+34_linux-x64_bin.tar.gz
# Sun, 02 Feb 2020 06:22:56 GMT
ENV JAVA_SHA256=51d9dd2161a912ab7bd2bf2e08043cdd175ce22b28608442e0d06bc777286158
# Sun, 02 Feb 2020 06:23:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Sun, 02 Feb 2020 06:23:23 GMT
CMD ["jshell"]
# Sun, 02 Feb 2020 21:43:21 GMT
ENV LEIN_VERSION=2.9.1
# Sun, 02 Feb 2020 21:43:21 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sun, 02 Feb 2020 21:43:22 GMT
WORKDIR /tmp
# Sun, 02 Feb 2020 21:43:29 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha1sum lein-pkg && echo "93be2c23ab4ff2fc4fcf531d7510ca4069b8d24a *lein-pkg" | sha1sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver pool.sks-keyservers.net --recv-key 2B72BF956E23DE5E830D50F6002AF007D1A7CC18 && echo "Verifying Jar file signature ..." && gpg --verify leiningen-$LEIN_VERSION-standalone.zip.asc && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get remove -y --purge gnupg wget
# Sun, 02 Feb 2020 21:43:30 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sun, 02 Feb 2020 21:43:30 GMT
ENV LEIN_ROOT=1
# Sun, 02 Feb 2020 21:43:34 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Sun, 02 Feb 2020 21:43:34 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d06863bb82bdc3f4cd17d49c0dee8720f91c4d9e40cce1b4a691f9459266be`  
		Last Modified: Sun, 02 Feb 2020 06:31:53 GMT  
		Size: 3.2 MB (3249109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3094a8803afb0148c3b1bb33abefbd6178d7e6fd2d074897735fbdcdc55ed4`  
		Last Modified: Sun, 02 Feb 2020 06:33:00 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2040ee43278f388deb957b072be36f7d1052eafb082ec91819c30df88e9dd4`  
		Last Modified: Sun, 02 Feb 2020 06:33:29 GMT  
		Size: 199.4 MB (199438691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1720f7bf3f531f0477b09050eeb68b0912bad82f2582c9fd788e027f2b0a06`  
		Last Modified: Sun, 02 Feb 2020 21:49:58 GMT  
		Size: 17.8 MB (17789375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5e890c611a6015477c025f6632f49c1183b76b524198afeadc02bf705dae7e`  
		Last Modified: Sun, 02 Feb 2020 21:49:57 GMT  
		Size: 4.2 MB (4168140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
