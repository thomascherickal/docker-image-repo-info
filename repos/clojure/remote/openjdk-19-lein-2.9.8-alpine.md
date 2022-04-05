## `clojure:openjdk-19-lein-2.9.8-alpine`

```console
$ docker pull clojure@sha256:1b3a0fc0a9eff3f66d985b3cf2396b1054dc1fcb9d54ecced43fa1c9cf98dcef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-19-lein-2.9.8-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:ad199fa22b5a6c1134521c8a83686af2202ddbf7b45a003c4f739a95db56ffb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.9 MB (210939046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d92c8d164299ccef82ab7bf04501cc5d230217061d7431dfc8e719f22330741`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:20:40 GMT
RUN apk add --no-cache java-cacerts
# Tue, 05 Apr 2022 10:20:40 GMT
ENV JAVA_HOME=/opt/openjdk-19
# Tue, 05 Apr 2022 10:20:40 GMT
ENV PATH=/opt/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 10:20:40 GMT
ENV JAVA_VERSION=19-ea+5
# Tue, 05 Apr 2022 10:20:51 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/5/binaries/openjdk-19-ea+5_linux-x64-musl_bin.tar.gz'; 			downloadSha256='0ee67a41fe97341f131bd4f065ed6092d55c15de5f00f8ba1e57d21eefb2c787'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 05 Apr 2022 10:20:51 GMT
CMD ["jshell"]
# Tue, 05 Apr 2022 15:59:14 GMT
ENV LEIN_VERSION=2.9.8
# Tue, 05 Apr 2022 15:59:14 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 05 Apr 2022 15:59:14 GMT
WORKDIR /tmp
# Tue, 05 Apr 2022 15:59:19 GMT
RUN set -eux; apk add --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "9952cba539cc6454c3b7385ebce57577087bf2b9001c3ab5c55d668d0aeff6e9 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Tue, 05 Apr 2022 15:59:19 GMT
ENV PATH=/opt/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 05 Apr 2022 15:59:20 GMT
ENV LEIN_ROOT=1
# Tue, 05 Apr 2022 15:59:24 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Tue, 05 Apr 2022 15:59:24 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Tue, 05 Apr 2022 15:59:24 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 05 Apr 2022 15:59:24 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652302906a15152c7ccbc20fb29082a3a6c23b32b20b1510eadc656e28474de8`  
		Last Modified: Tue, 05 Apr 2022 10:26:55 GMT  
		Size: 918.6 KB (918584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb589e67783e2a820d94ecc2fbc5976eabbacb7c7cdfe21d8195791f058c611`  
		Last Modified: Tue, 05 Apr 2022 10:27:09 GMT  
		Size: 190.6 MB (190592800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae592f19ffc30a8a757e05547287d77c132406f950ed9a7ae4fa1da0ee01ff`  
		Last Modified: Tue, 05 Apr 2022 16:05:08 GMT  
		Size: 12.4 MB (12405465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e235137190ea85b8313f3db9b2be5a013a5bea3cc4f6f83aec3ac53655d2b9`  
		Last Modified: Tue, 05 Apr 2022 16:05:07 GMT  
		Size: 4.2 MB (4207230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2cad33a00e6cc222820e000782d6b379b01ed5c7b61a5bfb2b2d13bb5d3fb1`  
		Last Modified: Tue, 05 Apr 2022 16:05:07 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
