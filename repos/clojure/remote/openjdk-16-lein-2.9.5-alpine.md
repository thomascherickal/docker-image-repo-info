## `clojure:openjdk-16-lein-2.9.5-alpine`

```console
$ docker pull clojure@sha256:9dd8a8623f047db232a46aa19be44080078516db05ed70e74bdfb56ea3bdf7cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-lein-2.9.5-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:2b0d957a56a78b9351bc65c6ca87910a2498e3c7465356c1f461f55c6bc90a17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.2 MB (206165925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb0dfa2a0542b3b67d9e21348f1f43f7e1eee9948ecdca6c5326735f92764cd2`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:15:27 GMT
RUN apk add --no-cache java-cacerts
# Thu, 17 Dec 2020 13:15:27 GMT
ENV JAVA_HOME=/opt/openjdk-16
# Thu, 17 Dec 2020 13:15:28 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Jan 2021 23:25:47 GMT
ENV JAVA_VERSION=16-ea+32
# Fri, 15 Jan 2021 23:26:43 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		x86_64) 			downloadUrl=https://download.java.net/java/early_access/alpine/32/binaries/openjdk-16-ea+32_linux-x64-musl_bin.tar.gz; 			downloadSha256=f9ec3071fdea08ca5be7b149d6c2f2689814e3ee86ee15b7981f5eed76280985; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 15 Jan 2021 23:26:44 GMT
CMD ["jshell"]
# Sat, 16 Jan 2021 01:30:26 GMT
ENV LEIN_VERSION=2.9.5
# Sat, 16 Jan 2021 01:30:26 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sat, 16 Jan 2021 01:30:27 GMT
WORKDIR /tmp
# Sat, 16 Jan 2021 01:30:30 GMT
RUN apk add --update --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Sat, 16 Jan 2021 01:30:30 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 16 Jan 2021 01:30:31 GMT
ENV LEIN_ROOT=1
# Sat, 16 Jan 2021 01:30:36 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Sat, 16 Jan 2021 01:30:36 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7f0194508bfdf90c2d4c810091723a528db557a8f15dc3342de6f146b13a31`  
		Last Modified: Thu, 17 Dec 2020 13:21:09 GMT  
		Size: 927.2 KB (927220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222cdd7f57af7ea33595647ef8743e8ab04a9785bffbcb340f2df213c0ff355f`  
		Last Modified: Fri, 15 Jan 2021 23:38:06 GMT  
		Size: 186.0 MB (185957831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d312d3e818d1ba3db68d1fd3a2fbf2937344327509ff26d7d5fa303f4cc08404`  
		Last Modified: Sat, 16 Jan 2021 01:36:04 GMT  
		Size: 12.3 MB (12301556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a9aebbf48a188ed75fb3b05c6f43066494892eaa9f9b97b699bdb517bc07e6`  
		Last Modified: Sat, 16 Jan 2021 01:36:04 GMT  
		Size: 4.2 MB (4180252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
