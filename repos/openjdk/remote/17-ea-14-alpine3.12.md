## `openjdk:17-ea-14-alpine3.12`

```console
$ docker pull openjdk@sha256:a1d32a8b214ff4676148950aead8c08ee997ee270acf227198874c037b2552c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:17-ea-14-alpine3.12` - linux; amd64

```console
$ docker pull openjdk@sha256:1a1e54603c843c0259dd6f7c1815cc44df6009fbeb1b5307f638b9b905c84817
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.5 MB (190525362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1975eece44a7a14601ee8b3ec02ffe2d2faed2889e71ef92e1fda84067c5e385`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:43:57 GMT
RUN apk add --no-cache java-cacerts
# Fri, 26 Mar 2021 05:43:57 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Fri, 26 Mar 2021 05:43:58 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 05:43:58 GMT
ENV JAVA_VERSION=17-ea+14
# Fri, 26 Mar 2021 05:44:08 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/14/binaries/openjdk-17-ea+14_linux-x64-musl_bin.tar.gz'; 			downloadSha256='f07a1ac921333dafac1cd886ad49600ce143be7efebd32e1a02599a8a0829dd4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Mar 2021 05:44:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206b60088bec17106b0d68572dabe2db4c1712bc15bfbbe7a37b966ff0eeee61`  
		Last Modified: Fri, 26 Mar 2021 05:52:25 GMT  
		Size: 927.4 KB (927381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2639b6a97a0187bf7437475502f2c8905e993d59e0b3b5765edce35af093ac08`  
		Last Modified: Fri, 26 Mar 2021 05:52:41 GMT  
		Size: 186.8 MB (186798219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
