## `openjdk:15-ea-10-jdk-alpine`

```console
$ docker pull openjdk@sha256:86f7c2faec906512498f984aa195bc4c0cfdf4a499f3c8aa805239fc0395d7f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:15-ea-10-jdk-alpine` - linux; amd64

```console
$ docker pull openjdk@sha256:dcf49dca88a163c614edf2ec5cd1e679eb7a7cba7f573d4b615d3a3929152640
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203592649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f9d59833b5fa9819e9467ca5e42f86c2dff123f5adbba34ddf9f5b0710a3ee3`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Mon, 22 Jun 2020 20:22:15 GMT
RUN apk add --no-cache java-cacerts
# Mon, 22 Jun 2020 20:22:15 GMT
ENV JAVA_HOME=/opt/openjdk-15
# Mon, 22 Jun 2020 20:22:15 GMT
ENV PATH=/opt/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 22 Jun 2020 20:22:16 GMT
ENV JAVA_VERSION=15-ea+10
# Mon, 22 Jun 2020 20:22:16 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/alpine/10/binaries/openjdk-15-ea+10_linux-x64-musl_bin.tar.gz
# Mon, 22 Jun 2020 20:22:16 GMT
ENV JAVA_SHA256=15a5e8002e24ed129b82bfe55ffe4bdbf3cfd0a7e5ad3399879cdd44175bfd06
# Mon, 22 Jun 2020 20:22:57 GMT
RUN set -eux; 		wget -O /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java --version; 	javac --version
# Mon, 22 Jun 2020 20:22:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0121b9d547c5ad1e5b9845b4a6b9f44a4bb6c15e45cc609316809d19b5d27345`  
		Last Modified: Mon, 22 Jun 2020 20:26:56 GMT  
		Size: 971.8 KB (971778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ae062329c82bbdb09eb9b3ac5a9f754a1a9a4d7ffb87a547ffbefccb4ed628`  
		Last Modified: Mon, 22 Jun 2020 20:27:13 GMT  
		Size: 199.8 MB (199807555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
