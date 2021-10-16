## `openjdk:18-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:39b81aedf8317884bcadf90add137cebe13cd367c3e0638b128141a60d9fd91f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:8d13c68184a932a4b9336ddefea5d6e378d45e52888a261b749dbc2ce28b71be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.5 MB (251548832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e78a5477e1962b520ad1eef910bc2d4bcf1c0461cc6310da23e456c7d329f7d`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 13 Oct 2021 18:30:19 GMT
ADD file:a6def617e1c0cf7def2d3ce3c79073621ed8efb37deed65fb49e7fc0a6d8ea37 in / 
# Wed, 13 Oct 2021 18:30:20 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 18:48:31 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 13 Oct 2021 18:48:31 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 13 Oct 2021 18:48:32 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 18:48:32 GMT
ENV LANG=en_US.UTF-8
# Sat, 16 Oct 2021 00:25:29 GMT
ENV JAVA_VERSION=18-ea+19
# Sat, 16 Oct 2021 00:25:39 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='42b5b8f65bed00be3fa810f876581eb1cd5eebcfe44dae0361e9f4128ec905cd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='518af06c8ba2d135a7ba43a937f1ed061e7d6acf55dc296cef60b1fd50413438'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Oct 2021 00:25:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e0ada0403966475cc22d4e65b5fd1bde8aac848d542317ef0154b8961c767d23`  
		Last Modified: Wed, 13 Oct 2021 18:31:57 GMT  
		Size: 48.2 MB (48235779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ebd61f33542411694b578674a48c8a09f401b78b67f813518bff7eb70dbbb`  
		Last Modified: Wed, 13 Oct 2021 18:57:37 GMT  
		Size: 15.4 MB (15397943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56561e197f344628210f6c9dc5cd0e8eb18a8be6a49286d952f75d2e8a0a6ecb`  
		Last Modified: Sat, 16 Oct 2021 00:33:13 GMT  
		Size: 187.9 MB (187915110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:e6488d21574f612580809adef1253608b0215a60aca9f157b37aa724aeff3067
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.1 MB (252104540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02521148fc03fee03cdbdb729383555ae92b29a0ccf4cfa1da361ed9e9d8fe6e`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 14 Oct 2021 03:43:46 GMT
ADD file:fca1474953cf608c9b2613787e7e7b859d458af91405a97dbd4ee57c63565185 in / 
# Thu, 14 Oct 2021 03:43:47 GMT
CMD ["/bin/bash"]
# Thu, 14 Oct 2021 05:43:29 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 14 Oct 2021 05:43:30 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 14 Oct 2021 05:43:31 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Oct 2021 05:43:32 GMT
ENV LANG=en_US.UTF-8
# Sat, 16 Oct 2021 00:05:39 GMT
ENV JAVA_VERSION=18-ea+19
# Sat, 16 Oct 2021 00:05:55 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='42b5b8f65bed00be3fa810f876581eb1cd5eebcfe44dae0361e9f4128ec905cd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='518af06c8ba2d135a7ba43a937f1ed061e7d6acf55dc296cef60b1fd50413438'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Oct 2021 00:05:56 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1322b24b1fa49fc9b6d0dad59ae623077ce5c89f6aca858053f6d7e45222e954`  
		Last Modified: Thu, 14 Oct 2021 03:45:17 GMT  
		Size: 48.8 MB (48820013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dfa211810869c7e6ae1a8fdb375623b16dc354d9e55dd50190c994ba3b3263`  
		Last Modified: Thu, 14 Oct 2021 05:58:58 GMT  
		Size: 16.4 MB (16447841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb7ede2a52f343cb2130ca3e22484f0633480adc7b27700588545ddfd6370c2`  
		Last Modified: Sat, 16 Oct 2021 00:18:58 GMT  
		Size: 186.8 MB (186836686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
