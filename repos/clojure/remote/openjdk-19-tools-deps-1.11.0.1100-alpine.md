## `clojure:openjdk-19-tools-deps-1.11.0.1100-alpine`

```console
$ docker pull clojure@sha256:470fdb8357bfa4216a23514ed184d453fb31306376025941ecbc843add29dfc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-19-tools-deps-1.11.0.1100-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:8ead1c8458c28c0d312c41d98770e809ebf71f89ec4ed8f7a825e6e5abf56846
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.2 MB (224160168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dd2414ce9ae8aaf85254b6dcad3d539e4914920a25d9abbeeba5b91650a9c93`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

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
# Tue, 05 Apr 2022 16:00:37 GMT
ENV CLOJURE_VERSION=1.11.0.1100
# Tue, 05 Apr 2022 16:00:37 GMT
WORKDIR /tmp
# Tue, 05 Apr 2022 16:00:43 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "a71bd520bd43d4be6e0cab0c525f5d1f85911fc276f3d0f37f00243fb0f1e594 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Tue, 05 Apr 2022 16:00:43 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Apr 2022 16:00:43 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 05 Apr 2022 16:00:43 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 05 Apr 2022 16:00:44 GMT
CMD ["-M" "--repl"]
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
	-	`sha256:1ca11c86888164c60f3cbcdd4d816d025a106c4e30ea46f841c57c68d7daddf8`  
		Last Modified: Tue, 05 Apr 2022 16:05:36 GMT  
		Size: 29.8 MB (29833195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1241576b4239404ff7505c11322bd02987390e80205c6c2c60b935567ee8f5`  
		Last Modified: Tue, 05 Apr 2022 16:05:34 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6b8452423dfb5a936267b5eab97e43531e70d3021bb0db8eb7f145ce54089f`  
		Last Modified: Tue, 05 Apr 2022 16:05:34 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
