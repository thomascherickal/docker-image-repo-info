## `openjdk:16-ea-oraclelinux8`

```console
$ docker pull openjdk@sha256:da80552ed501d0c57b2f387976629ebf5d3f4daed070665135e3cd32e5faf0b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-ea-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:0aaae979d688acfaaade5aca683c4a867d49aeb43763d4732c4b229bcce9a1d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.3 MB (264335540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18c6ff3936c8406bf053fb62b5a22a0451a10657105e4745182a12b04b6b0e2f`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Mon, 14 Sep 2020 18:33:21 GMT
ADD file:8011e31575cbf4b8ebb243821b300ba24330e02cab925024aa98f4ce27997846 in / 
# Mon, 14 Sep 2020 18:33:21 GMT
CMD ["/bin/bash"]
# Mon, 14 Sep 2020 18:50:46 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 14 Sep 2020 18:50:46 GMT
ENV LANG=C.UTF-8
# Mon, 14 Sep 2020 18:50:47 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Mon, 14 Sep 2020 18:50:47 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Sep 2020 18:50:47 GMT
ENV JAVA_VERSION=16-ea+15
# Mon, 14 Sep 2020 18:51:26 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/15/GPL/openjdk-16-ea+15_linux-aarch64_bin.tar.gz; 			downloadSha256=c0fda06a69e492907fe85d1e151e34747e0fce3a2221a70e5dcffd8df048d1db; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/15/GPL/openjdk-16-ea+15_linux-x64_bin.tar.gz; 			downloadSha256=7e6eccd3ac82ce7c007b30a8cde4d849c61612be5353de130690646814f5b9f9; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 14 Sep 2020 18:51:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:79701ada7495177c292979fd69d41eee91dc93ef0feea5ff95bb453f4ab7a1c5`  
		Last Modified: Mon, 14 Sep 2020 18:35:00 GMT  
		Size: 54.2 MB (54164063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffa6cd00cf525ae203ffe0f93764b5d175c46f27a7e15bb0da88efb308e5292`  
		Last Modified: Mon, 14 Sep 2020 18:55:41 GMT  
		Size: 13.5 MB (13491747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df66d4ae3f808f3e52b901fc18e1611b78dd0bb73469727cd4bfce720377b8f`  
		Last Modified: Mon, 14 Sep 2020 18:55:56 GMT  
		Size: 196.7 MB (196679730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-ea-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b531a2601a67e6863e1ee59b57704bf2fd5dcd5ccc550441d172df33f82b5c94
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.0 MB (244018719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1688401eb6474773d81af5ad61038030559b258eb78ad5959601136746e09c09`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 May 2019 21:40:52 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Mon, 14 Sep 2020 17:42:14 GMT
ADD file:b3bd5c2ec8ff0efe8a0b1384563b42f02d6bcf7531132d9ec4748ecfe264d476 in / 
# Mon, 14 Sep 2020 17:42:18 GMT
CMD ["/bin/bash"]
# Mon, 14 Sep 2020 17:59:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 14 Sep 2020 18:00:04 GMT
ENV LANG=C.UTF-8
# Mon, 14 Sep 2020 18:00:06 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Mon, 14 Sep 2020 18:00:07 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Sep 2020 18:00:07 GMT
ENV JAVA_VERSION=16-ea+15
# Mon, 14 Sep 2020 18:00:57 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/15/GPL/openjdk-16-ea+15_linux-aarch64_bin.tar.gz; 			downloadSha256=c0fda06a69e492907fe85d1e151e34747e0fce3a2221a70e5dcffd8df048d1db; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/15/GPL/openjdk-16-ea+15_linux-x64_bin.tar.gz; 			downloadSha256=7e6eccd3ac82ce7c007b30a8cde4d849c61612be5353de130690646814f5b9f9; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 14 Sep 2020 18:01:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a805b9845b615e5963d09def3e5e9919b39e76b5122c2abecc98d4a4bb358394`  
		Last Modified: Mon, 14 Sep 2020 17:43:27 GMT  
		Size: 54.3 MB (54266593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dee2ba14d3dd42ac318a14c434bced8bd3cc7a2c58339deb209699b1d167b21`  
		Last Modified: Mon, 14 Sep 2020 20:56:35 GMT  
		Size: 14.4 MB (14366836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d8e66a354b59ebdd090ba036a67e82f1ca3441e6e50da045ca773c2a546dbe`  
		Last Modified: Mon, 14 Sep 2020 20:56:59 GMT  
		Size: 175.4 MB (175385290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
