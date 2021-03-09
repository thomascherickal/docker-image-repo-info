## `clojure:openjdk-17-boot-2.8.3-alpine`

```console
$ docker pull clojure@sha256:eda79403a08daea61bc03b39843269f167593bb1e0778f1bc65e58402b6fabe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-17-boot-2.8.3-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:439156b555e664a91dc70dc657fbdf3578f6b0e026c9c72148b4260b4c8953d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.3 MB (250278520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:499afca9543039a57c7187fde5aed5f9444f29378526d83587f6d93f74c89441`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 20:57:21 GMT
RUN apk add --no-cache java-cacerts
# Tue, 09 Mar 2021 20:57:21 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Tue, 09 Mar 2021 20:57:21 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:57:21 GMT
ENV JAVA_VERSION=17-ea+10
# Tue, 09 Mar 2021 20:58:11 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/10/binaries/openjdk-17-ea+10_linux-x64-musl_bin.tar.gz'; 			downloadSha256='fc3ea4225030a5df6191b6027051e705e6c34b72115dfdb36d170d735cb409d5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 20:58:11 GMT
CMD ["jshell"]
# Tue, 09 Mar 2021 21:55:11 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 09 Mar 2021 21:55:12 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 09 Mar 2021 21:55:12 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:55:13 GMT
RUN apk add --update --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Tue, 09 Mar 2021 21:55:14 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 09 Mar 2021 21:55:14 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 09 Mar 2021 21:55:33 GMT
RUN boot
# Tue, 09 Mar 2021 21:55:33 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b1e51638093d53268f8affa33c76d79b5f585556917511babcc02780047d7b`  
		Last Modified: Tue, 09 Mar 2021 21:11:38 GMT  
		Size: 928.4 KB (928404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fccea66d261db26595f6c615d2361af9b26994c460c6b0736185a09e1cb602a`  
		Last Modified: Tue, 09 Mar 2021 21:11:53 GMT  
		Size: 186.9 MB (186889693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ca7bb751e97a0925b658ae97b107fd9b112b1dba0572b4d8fd6796811470d0`  
		Last Modified: Tue, 09 Mar 2021 22:11:01 GMT  
		Size: 828.4 KB (828424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072d82751cfde1ee122052b122ed6770b5e70bda4a0b784cd44c9a18cef394b1`  
		Last Modified: Tue, 09 Mar 2021 22:11:04 GMT  
		Size: 58.8 MB (58820342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
