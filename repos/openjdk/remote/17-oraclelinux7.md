## `openjdk:17-oraclelinux7`

```console
$ docker pull openjdk@sha256:033961f74da45a145069c919e6ce23c28374aec3ec01ee42990073813f4b3c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:9ac1648f9f22f9fa75a46f6397efec7d526d04aacca75e8542666b51728efe09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249581291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b17c2729fe99584e15bad04a404e9ddba1fbe21d8bd6492ef42a3fec27c0b7cf`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 15 Jan 2021 00:31:31 GMT
ADD file:dee09ad1ed4e7359b14fabc84890b1fb687ad4efe75f7c4800c0a907fd4f70a3 in / 
# Fri, 15 Jan 2021 00:31:32 GMT
CMD ["/bin/bash"]
# Fri, 15 Jan 2021 00:58:14 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 15 Jan 2021 00:58:14 GMT
ENV LANG=en_US.UTF-8
# Fri, 15 Jan 2021 00:58:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 15 Jan 2021 00:58:15 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Jan 2021 00:58:15 GMT
ENV JAVA_VERSION=17-ea+4
# Fri, 15 Jan 2021 00:58:55 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk17/4/GPL/openjdk-17-ea+4_linux-aarch64_bin.tar.gz; 			downloadSha256=fbe659e6dc6b9920cc39719cdfe25cb84215d7fd584b5d417916292329305050; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk17/4/GPL/openjdk-17-ea+4_linux-x64_bin.tar.gz; 			downloadSha256=5872e34f20279f586e1a3cfb9410043f202455306afd4b33dc660d43f8693998; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 15 Jan 2021 00:58:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:980316e412373040bc280150078ae453b259ece36b750a0a9b6f4c99751ce4f9`  
		Last Modified: Wed, 06 Jan 2021 20:24:02 GMT  
		Size: 48.3 MB (48260808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7699f318b6b854fb950c083e0fed757fff0549df020432861c6b50802ec82b2`  
		Last Modified: Fri, 15 Jan 2021 01:09:18 GMT  
		Size: 15.4 MB (15431689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94be6f3ab8d9de2b5b62727a6517cc2c4c52533909c3ad804c92d50adc7f6a4`  
		Last Modified: Fri, 15 Jan 2021 01:09:36 GMT  
		Size: 185.9 MB (185888794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:78a3e50fc317a94249d89fdda98ce471dd37d3fdfb97c8bbd9a4e30fd66f4066
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.6 MB (245570727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa155e9c43dcb7f4f7cba54bcdc4f758d70d5bf628abce9e7334cb3c86b253c8`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 15 Jan 2021 00:06:30 GMT
ADD file:d4d5ffcc8d57e27f8de10063c4e347d2f4da299f62166d6f6387a7714f5e0f06 in / 
# Fri, 15 Jan 2021 00:06:33 GMT
CMD ["/bin/bash"]
# Fri, 15 Jan 2021 00:45:52 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 15 Jan 2021 00:45:53 GMT
ENV LANG=en_US.UTF-8
# Fri, 15 Jan 2021 00:45:54 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 15 Jan 2021 00:45:55 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Jan 2021 22:46:36 GMT
ENV JAVA_VERSION=17-ea+5
# Fri, 15 Jan 2021 22:46:59 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk17/5/GPL/openjdk-17-ea+5_linux-aarch64_bin.tar.gz; 			downloadSha256=5320fe7df7906893dc060984832ade284ffbe9cf767e4428e628cf517b1b0a92; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk17/5/GPL/openjdk-17-ea+5_linux-x64_bin.tar.gz; 			downloadSha256=0de74da4de6dfd013fad9b1c121b58568128117d3e9ac66508b05b46ebbdce1d; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 15 Jan 2021 22:47:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e2e87614faabf530f11811ae8eb1be9e586d5d923036268129a39eae319cb772`  
		Last Modified: Wed, 06 Jan 2021 20:47:54 GMT  
		Size: 48.9 MB (48858154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458e99ea3b1687330632146091a5677b179fe906820e2d98ad7b5becbcb526c1`  
		Last Modified: Fri, 15 Jan 2021 00:56:17 GMT  
		Size: 16.5 MB (16470870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91e1a9fd2273c77fbfff39d718cfd0166c735934033ebf35e824aa0cb4d377b`  
		Last Modified: Fri, 15 Jan 2021 22:56:40 GMT  
		Size: 180.2 MB (180241703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
