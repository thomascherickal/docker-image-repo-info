## `clojure:openjdk-16-alpine`

```console
$ docker pull clojure@sha256:158994f80de0992a94d8e1b8906679df866042c5d9ba27fd350fea20eae62166
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:11de30211aa5e53eb6dc129413eae2aece36cfffc0f65479f1ddcb01ec18af3f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.5 MB (219528360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd690bac2932aada861153b203d020c9256fa5b61179cacaa6d43842410d8e7b`
-	Default Command: `["lein","repl"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 01:05:44 GMT
RUN apk add --no-cache java-cacerts
# Wed, 22 Jul 2020 01:05:44 GMT
ENV JAVA_HOME=/opt/openjdk-16
# Wed, 22 Jul 2020 01:05:45 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Oct 2020 22:42:25 GMT
ENV JAVA_VERSION=16-ea+14
# Tue, 06 Oct 2020 22:43:05 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		x86_64) 			downloadUrl=https://download.java.net/java/early_access/alpine/14/binaries/openjdk-16-ea+14_linux-x64-musl_bin.tar.gz; 			downloadSha256=6d6943f9c350ca20fd2892e024c363e538ab4a2c1aeaceeab4450a47cbaca54c; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 06 Oct 2020 22:43:05 GMT
CMD ["jshell"]
# Tue, 06 Oct 2020 23:04:41 GMT
ENV LEIN_VERSION=2.9.3
# Tue, 06 Oct 2020 23:04:41 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 06 Oct 2020 23:04:42 GMT
WORKDIR /tmp
# Tue, 06 Oct 2020 23:04:45 GMT
RUN apk add --update --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "42e18e8a833b863ddfba1c5565bd5d78b54bcee661ec86e94a8bdc67b1733e63 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Tue, 06 Oct 2020 23:04:45 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Oct 2020 23:04:46 GMT
ENV LEIN_ROOT=1
# Tue, 06 Oct 2020 23:04:49 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 06 Oct 2020 23:04:50 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a2e4aad8c98294e53534e7aef0572d7a04cc37264f1b4b75d0878244e59c7f`  
		Last Modified: Wed, 22 Jul 2020 01:13:01 GMT  
		Size: 926.4 KB (926401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e805847a3f5a367d2dc07f7d593bfc29d8aeef68dcf5e0248810317802765aac`  
		Last Modified: Tue, 06 Oct 2020 22:46:40 GMT  
		Size: 197.7 MB (197669352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4cdded2bd124dd62732178b4586be1bbcaee9f48ca2b0c7e247410c7086a9a`  
		Last Modified: Tue, 06 Oct 2020 23:06:57 GMT  
		Size: 14.0 MB (13966851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e108f3bd782e53aa4e0f8bbf9f1f89b1d4596bd307ed28fe74dca96361f9aef`  
		Last Modified: Tue, 06 Oct 2020 23:06:57 GMT  
		Size: 4.2 MB (4168215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
