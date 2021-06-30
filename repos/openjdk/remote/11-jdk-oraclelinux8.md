## `openjdk:11-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:ddb1de39c73130e1df9da5877abbe23aff0564e7383ce02700196dcbe1d6dc8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:11-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:9815631398c1753c6d01ce226485f3a0e141946caed6f0301ff2c51000921c7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258388147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95cfb60ac29ca734a777ea996b36bba7da35aeb30f84edc5373ba35c01856bbc`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 30 Jun 2021 17:23:40 GMT
ADD file:d49890823c4e8287f936eec210400575f79c20f14f048017368faed0584841a6 in / 
# Wed, 30 Jun 2021 17:23:41 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 17:40:57 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Jun 2021 17:44:55 GMT
ENV JAVA_HOME=/usr/java/openjdk-11
# Wed, 30 Jun 2021 17:44:55 GMT
ENV PATH=/usr/java/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Jun 2021 17:44:55 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 17:44:56 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 30 Jun 2021 17:45:14 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_linux_11.0.11_9.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 30 Jun 2021 17:45:15 GMT
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
	-	`sha256:b81132381c62eb6e71742dc6bc456d7a7ca03c69a6317948495ed43700748219`  
		Last Modified: Wed, 30 Jun 2021 17:53:48 GMT  
		Size: 202.8 MB (202817474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:e880422268f36fc555e8f87bda33939ea4f7aac5467a209af6ef2331ff8b8388
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.7 MB (256661039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4c24125fa3688d1558bfb1d7affacc5454e407b157afcaaaf4ca2c7b998f00`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 30 Jun 2021 16:40:33 GMT
ADD file:c33580f17660c9afa2637bda7e6cf34d631535b13ffc1535bb21cfb0ab7bdb5c in / 
# Wed, 30 Jun 2021 16:40:33 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 17:08:45 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Jun 2021 17:11:26 GMT
ENV JAVA_HOME=/usr/java/openjdk-11
# Wed, 30 Jun 2021 17:11:26 GMT
ENV PATH=/usr/java/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Jun 2021 17:11:26 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 17:11:26 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 30 Jun 2021 17:11:40 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_linux_11.0.11_9.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 30 Jun 2021 17:11:41 GMT
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
	-	`sha256:77e4e2cbdc3f88efe03bb0b3b97cf064a00403842ed6516f57605182c2a8cd65`  
		Last Modified: Wed, 30 Jun 2021 17:26:01 GMT  
		Size: 200.4 MB (200436491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
