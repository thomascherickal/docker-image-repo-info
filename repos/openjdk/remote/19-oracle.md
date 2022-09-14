## `openjdk:19-oracle`

```console
$ docker pull openjdk@sha256:a5f2327c217367af3729670628c7ad66799cd890bde4e14fad02c2ae59552424
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:973fe414a4e1f3e41e291b068183684a88827dd2cb5f78214da26632d5218702
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (249006200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6f6690e479ce4ad3600d1b87ff79ea5dc6438165902f332ab7f721f7599c6b`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 14 Sep 2022 21:20:28 GMT
ADD file:e00d9d8d8f616feec8c064f2250e4836ea3b533ead0611d1af2245974abb4e88 in / 
# Wed, 14 Sep 2022 21:20:28 GMT
CMD ["/bin/bash"]
# Wed, 14 Sep 2022 21:37:14 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 14 Sep 2022 21:37:46 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Wed, 14 Sep 2022 21:37:46 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Sep 2022 21:37:46 GMT
ENV LANG=C.UTF-8
# Wed, 14 Sep 2022 21:37:46 GMT
ENV JAVA_VERSION=19
# Wed, 14 Sep 2022 21:37:58 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk19/877d6127e982470ba2a7faa31cc93d04/36/GPL/openjdk-19_linux-x64_bin.tar.gz'; 			downloadSha256='f47aba585cfc9ecff1ed8e023524e8309f4315ed8b80100b40c7dcc232c12f96'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk19/877d6127e982470ba2a7faa31cc93d04/36/GPL/openjdk-19_linux-aarch64_bin.tar.gz'; 			downloadSha256='682bfb48158ca198393c4b7fd38f873e8d6316b0bc6511a07e917f7f0f3afb03'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 14 Sep 2022 21:37:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:051f419db9dd9462e8995886d24f592c26cef792cc915dfbc7548e0b19aa55fe`  
		Last Modified: Wed, 14 Sep 2022 21:21:25 GMT  
		Size: 40.6 MB (40590248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa51c6010a14c1984cbdea1332a5d2f77bf6e0141bc497b44dca611e21f9b391`  
		Last Modified: Wed, 14 Sep 2022 21:41:16 GMT  
		Size: 12.2 MB (12232427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba785fff917fb7bc8692503ac810691754ab0f6e0cdfbf4941b0de2305ab652`  
		Last Modified: Wed, 14 Sep 2022 21:42:33 GMT  
		Size: 196.2 MB (196183525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b9a5ae2ba813e56f745e5de4381de18e89737ee3850e7936a36919ee1a5f6e15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.5 MB (247489639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fafed7e8bf172ded4c7281bf750a9a3a4fd9fe1718f94f179a3edeae8e36491c`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 14 Sep 2022 21:41:16 GMT
ADD file:30401488699aa4b911abaeec83f0938e0fede937c09940369ec58cc56eae4624 in / 
# Wed, 14 Sep 2022 21:41:17 GMT
CMD ["/bin/bash"]
# Wed, 14 Sep 2022 22:01:28 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 14 Sep 2022 22:02:31 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Wed, 14 Sep 2022 22:02:32 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Sep 2022 22:02:33 GMT
ENV LANG=C.UTF-8
# Wed, 14 Sep 2022 22:02:34 GMT
ENV JAVA_VERSION=19
# Wed, 14 Sep 2022 22:02:47 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk19/877d6127e982470ba2a7faa31cc93d04/36/GPL/openjdk-19_linux-x64_bin.tar.gz'; 			downloadSha256='f47aba585cfc9ecff1ed8e023524e8309f4315ed8b80100b40c7dcc232c12f96'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk19/877d6127e982470ba2a7faa31cc93d04/36/GPL/openjdk-19_linux-aarch64_bin.tar.gz'; 			downloadSha256='682bfb48158ca198393c4b7fd38f873e8d6316b0bc6511a07e917f7f0f3afb03'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 14 Sep 2022 22:02:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9a8b791677e1fdf76ff862b55362355b48c8636d0eabf606d1af65888ab73ec8`  
		Last Modified: Wed, 14 Sep 2022 21:42:22 GMT  
		Size: 39.4 MB (39409909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1458b25adde8441e97a5f07c35975478bc0d77410ada29b87b31f52fbbaf994`  
		Last Modified: Wed, 14 Sep 2022 22:09:27 GMT  
		Size: 13.1 MB (13055052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61531557699b2fbfe3d3e0904dcf753c8d0cbdd7effaca97b1310486d5837e13`  
		Last Modified: Wed, 14 Sep 2022 22:11:11 GMT  
		Size: 195.0 MB (195024678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
