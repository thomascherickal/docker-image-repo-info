## `clojure:openjdk-16-boot-2.8.3-alpine`

```console
$ docker pull clojure@sha256:d9371dfe81de830ccb28002aea3ae69cd7613e04053f61a242b95a2fa77afd9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-boot-2.8.3-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:0ffb4223ed6bab3d86a32ec31a881ca634f8d081eb55b4886abf3e47fb14e7df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.3 MB (249296733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5886beb9791b1553467dd3ebb5c340eea004261707c86666127ef0418df88d82`
-	Default Command: `["boot","repl"]`

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
# Sat, 16 Jan 2021 01:30:40 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 16 Jan 2021 01:30:40 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 16 Jan 2021 01:30:41 GMT
WORKDIR /tmp
# Sat, 16 Jan 2021 01:30:42 GMT
RUN apk add --update --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Sat, 16 Jan 2021 01:30:43 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 16 Jan 2021 01:30:43 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 16 Jan 2021 01:31:06 GMT
RUN boot
# Sat, 16 Jan 2021 01:31:06 GMT
CMD ["boot" "repl"]
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
	-	`sha256:c827e8bfeea853818d8261c2b6c7f0ed5f5fbe6f60e73105d614a003eff37bd4`  
		Last Modified: Sat, 16 Jan 2021 01:36:13 GMT  
		Size: 792.3 KB (792335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bb1a7c925df82dc378c7437533fe322dbf6069f39d16523e6296696b413f47`  
		Last Modified: Sat, 16 Jan 2021 01:36:17 GMT  
		Size: 58.8 MB (58820281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
