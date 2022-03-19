## `clojure:openjdk-19-lein-2.9.8-alpine`

```console
$ docker pull clojure@sha256:45d40eb0a83e5c970a39f7a6de367486427ff5666b6fed4500d1c2173e1cdbd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-19-lein-2.9.8-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:8e8d03209cc46233e6832f68ee56e9feabb6c62384afab4f785cecb81044c5a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.9 MB (210937110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a6f2e4e7ca80719ab5ca7462f91f0ae45ebcf9bd00695fc2f5e5cd48e70edfb`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:09:32 GMT
RUN apk add --no-cache java-cacerts
# Thu, 17 Mar 2022 18:09:32 GMT
ENV JAVA_HOME=/opt/openjdk-19
# Thu, 17 Mar 2022 18:09:32 GMT
ENV PATH=/opt/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 18:09:32 GMT
ENV JAVA_VERSION=19-ea+5
# Thu, 17 Mar 2022 18:09:44 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/5/binaries/openjdk-19-ea+5_linux-x64-musl_bin.tar.gz'; 			downloadSha256='0ee67a41fe97341f131bd4f065ed6092d55c15de5f00f8ba1e57d21eefb2c787'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Mar 2022 18:09:45 GMT
CMD ["jshell"]
# Sat, 19 Mar 2022 11:13:48 GMT
ENV LEIN_VERSION=2.9.8
# Sat, 19 Mar 2022 11:13:48 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sat, 19 Mar 2022 11:13:48 GMT
WORKDIR /tmp
# Sat, 19 Mar 2022 11:13:52 GMT
RUN set -eux; apk add --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "9952cba539cc6454c3b7385ebce57577087bf2b9001c3ab5c55d668d0aeff6e9 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Sat, 19 Mar 2022 11:13:52 GMT
ENV PATH=/opt/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 19 Mar 2022 11:13:52 GMT
ENV LEIN_ROOT=1
# Sat, 19 Mar 2022 11:13:55 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Sat, 19 Mar 2022 11:13:56 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Sat, 19 Mar 2022 11:13:56 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 19 Mar 2022 11:13:56 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95bfa6190a5f1e660dfa661cfeacb195395e181263c1cccbc3920ee6ca80bbd`  
		Last Modified: Thu, 17 Mar 2022 18:26:15 GMT  
		Size: 918.6 KB (918586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79afb24595e792b2b9730c2c5afe2d3318709911a025123e55d49e217ce392f1`  
		Last Modified: Thu, 17 Mar 2022 18:26:30 GMT  
		Size: 190.6 MB (190592804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3780accbf1b2745c1641b832478c4fccb3641c87047a9ddac3143498095029`  
		Last Modified: Sat, 19 Mar 2022 11:33:46 GMT  
		Size: 12.4 MB (12405454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfa4215169fce6b2d42ef2c6fc51cfab02829d125c11bc9b0301c2f7b70ebdf`  
		Last Modified: Sat, 19 Mar 2022 11:33:45 GMT  
		Size: 4.2 MB (4207224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e06b1d28ad8af44abdb3f83c970968701f80eca4c11db7011a4f0b254b852`  
		Last Modified: Sat, 19 Mar 2022 11:33:45 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
