## `openjdk:16-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:04cb305dc4665f01f0a812505d60675cfa047a49f9280b1034afc871b5a008ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:c4185234bd34ce83dba9625ee4c5dd43df9ac1b064360f18418c9afadb707f05
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.4 MB (240370198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f1dadedfab6ad53f8b9ac935213173a718e015e96253e02101d7180d83a1b4`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 30 Jun 2021 17:23:40 GMT
ADD file:d49890823c4e8287f936eec210400575f79c20f14f048017368faed0584841a6 in / 
# Wed, 30 Jun 2021 17:23:41 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 17:40:57 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Jun 2021 17:44:02 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Wed, 30 Jun 2021 17:44:03 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Jun 2021 17:44:03 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 17:44:04 GMT
ENV JAVA_VERSION=16.0.1
# Wed, 30 Jun 2021 17:44:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='b1198ffffb7d26a3fdedc0fa599f60a0d12aa60da1714b56c1defbce95d8b235'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='602b005074777df2a0b4306e20152a6446803edd87ccbab95b2f313c4d9be6ba'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 30 Jun 2021 17:44:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9660ffb7976c51eb47b4425f6bb95173c170f4fcc442a2bb2b6ba7bf154f6fc8`  
		Last Modified: Wed, 30 Jun 2021 17:25:00 GMT  
		Size: 42.2 MB (42179226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f8b4ca74ea5f238671d4c7981ca7c99e6c70d3fcd8d4d0596ccdf6b8329dbe`  
		Last Modified: Wed, 30 Jun 2021 17:50:04 GMT  
		Size: 13.4 MB (13391447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9cb8f68ad4213ef62d6554e599eca648dd5b6c37f0771cead814a0590e4f50`  
		Last Modified: Wed, 30 Jun 2021 17:52:31 GMT  
		Size: 184.8 MB (184799525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:97c33d111e0f7459a831eaa64e73a260789422d218fb5ba42212ebf24bcbf80f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.4 MB (235404768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad25742264dbedb501090af5d41b4943c16a5894b9c920376c6067b7d56d4a3d`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 30 Jun 2021 16:40:33 GMT
ADD file:c33580f17660c9afa2637bda7e6cf34d631535b13ffc1535bb21cfb0ab7bdb5c in / 
# Wed, 30 Jun 2021 16:40:33 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 17:08:45 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Jun 2021 17:10:30 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Wed, 30 Jun 2021 17:10:30 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Jun 2021 17:10:31 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 17:10:31 GMT
ENV JAVA_VERSION=16.0.1
# Wed, 30 Jun 2021 17:10:40 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='b1198ffffb7d26a3fdedc0fa599f60a0d12aa60da1714b56c1defbce95d8b235'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='602b005074777df2a0b4306e20152a6446803edd87ccbab95b2f313c4d9be6ba'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 30 Jun 2021 17:10:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e02c40d2e97c148eec83200018cd774bcf09562d984b2237577a0bebd5900481`  
		Last Modified: Wed, 30 Jun 2021 16:41:47 GMT  
		Size: 42.0 MB (42045297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c341a81c74999386f57f0e8e08448131a5297ce89816bbfe58e5d804b6e1384`  
		Last Modified: Wed, 30 Jun 2021 17:21:19 GMT  
		Size: 14.2 MB (14179251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed10225377ef4e88417d458930319164fddd12bee5160fe482c50bc03a429ca`  
		Last Modified: Wed, 30 Jun 2021 17:24:18 GMT  
		Size: 179.2 MB (179180220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
