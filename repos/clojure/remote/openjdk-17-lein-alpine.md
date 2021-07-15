## `clojure:openjdk-17-lein-alpine`

```console
$ docker pull clojure@sha256:e6f4b3bbebee85272c8b431ccedd1f8e7781a388d0d524a5d7a33eed67207ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-17-lein-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:e99f5fad34b613234d36dcc502193cb27d939b58341ac41118906c31c5326738
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.1 MB (207083799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ebc89dbaf007ded6e035a1defd4b2e12009c458ea3ce54f3e380a68f3b10b7b`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Tue, 22 Jun 2021 21:40:57 GMT
RUN apk add --no-cache java-cacerts
# Tue, 22 Jun 2021 21:40:57 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Tue, 22 Jun 2021 21:40:57 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Jun 2021 21:40:58 GMT
ENV JAVA_VERSION=17-ea+14
# Tue, 22 Jun 2021 21:41:09 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/14/binaries/openjdk-17-ea+14_linux-x64-musl_bin.tar.gz'; 			downloadSha256='f07a1ac921333dafac1cd886ad49600ce143be7efebd32e1a02599a8a0829dd4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 22 Jun 2021 21:41:09 GMT
CMD ["jshell"]
# Tue, 22 Jun 2021 22:20:29 GMT
ENV LEIN_VERSION=2.9.6
# Tue, 22 Jun 2021 22:20:30 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 22 Jun 2021 22:20:30 GMT
WORKDIR /tmp
# Tue, 22 Jun 2021 22:20:35 GMT
RUN apk add --update --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Tue, 22 Jun 2021 22:20:35 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 22 Jun 2021 22:20:35 GMT
ENV LEIN_ROOT=1
# Tue, 22 Jun 2021 22:20:38 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Tue, 22 Jun 2021 22:20:39 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c9466125e464fed5626bde7b7a0f91aab09905f0a07e9ad4e930ae72e0fc63`  
		Last Modified: Tue, 22 Jun 2021 21:51:51 GMT  
		Size: 928.4 KB (928436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d715783b80cab158f5bf9726bcada5265c1624b64ca2bb46f42f94998d4662`  
		Last Modified: Tue, 22 Jun 2021 21:52:05 GMT  
		Size: 186.8 MB (186798299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f6ca8ab20ed84b46954e437c9b24eb573559982aba8c586010b4a932f449cb`  
		Last Modified: Tue, 22 Jun 2021 22:25:12 GMT  
		Size: 12.3 MB (12341863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1406dee28f766b29032d2580d3cbb0dc75f4ab9e1b585a03113eeeec2acaa326`  
		Last Modified: Tue, 22 Jun 2021 22:25:12 GMT  
		Size: 4.2 MB (4203723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
