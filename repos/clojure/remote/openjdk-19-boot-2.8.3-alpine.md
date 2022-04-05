## `clojure:openjdk-19-boot-2.8.3-alpine`

```console
$ docker pull clojure@sha256:8ed32804acc5218ab4bbf18b05c24161b54bf38ec437f2752c0aece16925eda7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-19-boot-2.8.3-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:552358e59e14b09d1ee325df671c4c17c78b7463275f67c8533c5bff0ff9e376
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.0 MB (253979046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132c7d00cd8d4d549bb9129a9aee07bb46e85fdb4731aa18c86132da433f67d9`
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
# Tue, 05 Apr 2022 15:59:28 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 05 Apr 2022 15:59:28 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 05 Apr 2022 15:59:28 GMT
WORKDIR /tmp
# Tue, 05 Apr 2022 15:59:29 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Tue, 05 Apr 2022 15:59:29 GMT
ENV PATH=/opt/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 05 Apr 2022 15:59:29 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 05 Apr 2022 16:00:31 GMT
RUN boot
# Tue, 05 Apr 2022 16:00:31 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 05 Apr 2022 16:00:31 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 05 Apr 2022 16:00:31 GMT
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
	-	`sha256:6a3ba863b8fe0c9dd5c748810c170eb543ed56f9ac47121c781185f18b222aee`  
		Last Modified: Tue, 05 Apr 2022 16:05:18 GMT  
		Size: 831.3 KB (831336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65651d301531371c6897a3564bc5585bb2e801d491c96b304faf4e4e8ef95527`  
		Last Modified: Tue, 05 Apr 2022 16:05:24 GMT  
		Size: 58.8 MB (58821362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22df4344142c25902a5d02e5cbdc310dabaeafedf6134c8caa0fbd869eac74e0`  
		Last Modified: Tue, 05 Apr 2022 16:05:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
