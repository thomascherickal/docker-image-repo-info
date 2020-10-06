## `clojure:openjdk-16-boot-2.8.3-alpine`

```console
$ docker pull clojure@sha256:c9a5dbcc9c2b907af71237f9c1fdf80c951caed57f42e4dbe87653b990756777
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-boot-2.8.3-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:c0bf590e0d7e00ea9e06592c8659df8c3fc0fbf8a48147033417c0c901d5d56f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (261005562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1586fe2f369a2b2449305577efb8e2d8f6e6edcb3ccccbaa74a936469a8288ea`
-	Default Command: `["boot","repl"]`

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
# Tue, 06 Oct 2020 23:04:54 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Oct 2020 23:04:54 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Oct 2020 23:04:54 GMT
WORKDIR /tmp
# Tue, 06 Oct 2020 23:04:55 GMT
RUN apk add --update --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Tue, 06 Oct 2020 23:04:55 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Oct 2020 23:04:56 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Oct 2020 23:05:14 GMT
RUN boot
# Tue, 06 Oct 2020 23:05:15 GMT
CMD ["boot" "repl"]
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
	-	`sha256:525bd467ac903f13e90a89b476b8aedf8fc3d2a5abff4a5a049a3d25f475cea0`  
		Last Modified: Tue, 06 Oct 2020 23:07:03 GMT  
		Size: 792.3 KB (792323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c57e7a62e930e21da665181aabb51893b55a06a46909820aeecad6fd1a87689`  
		Last Modified: Tue, 06 Oct 2020 23:07:10 GMT  
		Size: 58.8 MB (58819945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
