## `openjdk:20-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:fa5551b2c03dcf57823238a4ad5f94c8ed71e331ddc826d50a53f300d49d9b3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:ee8322c5a1b312d57b65f6b31b945eb8716376471ac61a71ec08cfc87e1fc599
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.8 MB (259819473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db0c174c7144cda7a71bcd5dab43e927159725625443fb5ad2528aa4f2aa230c`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 Aug 2022 19:35:42 GMT
ADD file:adf7ebc1d65494dba22f4f0a12f2f8f63128836b87646ffd6e9964f936343e6d in / 
# Wed, 24 Aug 2022 19:35:43 GMT
CMD ["/bin/bash"]
# Wed, 24 Aug 2022 22:44:32 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 24 Aug 2022 22:44:32 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 24 Aug 2022 22:44:32 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 22:44:33 GMT
ENV LANG=en_US.UTF-8
# Wed, 21 Sep 2022 00:00:32 GMT
ENV JAVA_VERSION=20-ea+15
# Wed, 21 Sep 2022 00:00:43 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='2ee417bc5d9f36c634a5e004c201967b70b6b3a5382147d74406cc9b015eac97'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='6ec219647905af892891d6fd018538043bf19cfae2a40df439b9fde070476681'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Sep 2022 00:00:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9815334b7810943f0c417fa41a2732d56b098252185c5749c2c2ce80f8e8e140`  
		Last Modified: Wed, 24 Aug 2022 19:37:41 GMT  
		Size: 48.7 MB (48727120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbb6577271d2ea4eb7961ad553fcac407890cd27f6514b5d071119191d585fd`  
		Last Modified: Wed, 24 Aug 2022 22:49:44 GMT  
		Size: 14.2 MB (14230815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49213efb36c47df660e37d8fbc7706d6b59343fbb6bfa87d45deddb12c7a7bc2`  
		Last Modified: Wed, 21 Sep 2022 00:05:17 GMT  
		Size: 196.9 MB (196861538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b4835832939c15b901c13e833dc451dcadaeaa5f041df8ddcd5bf1868ceca8ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.0 MB (259965228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcda8395f1f8c94d193bdeca61e8b6e5dbd1207ff70dff0a64bf8e66c888606c`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 Aug 2022 19:55:21 GMT
ADD file:58b53a780a05a9f314e6821fd85f38a0d86fed5a98ab7c3fd52b0ea2341c3d64 in / 
# Wed, 24 Aug 2022 19:55:22 GMT
CMD ["/bin/bash"]
# Wed, 24 Aug 2022 23:31:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 24 Aug 2022 23:31:54 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 24 Aug 2022 23:31:55 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 23:31:56 GMT
ENV LANG=en_US.UTF-8
# Wed, 21 Sep 2022 00:33:43 GMT
ENV JAVA_VERSION=20-ea+15
# Wed, 21 Sep 2022 00:34:06 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='2ee417bc5d9f36c634a5e004c201967b70b6b3a5382147d74406cc9b015eac97'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='6ec219647905af892891d6fd018538043bf19cfae2a40df439b9fde070476681'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Sep 2022 00:34:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9d094a37c2b34cb4c876f39d579c422eba5a195ec17dff5a5fcbbbd9398dafef`  
		Last Modified: Wed, 24 Aug 2022 19:57:30 GMT  
		Size: 49.3 MB (49309770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346cd8d935004b602845ed18ab7ddf7b6bf15cfcb9eb50d1b98f6153c188f3a3`  
		Last Modified: Wed, 24 Aug 2022 23:41:46 GMT  
		Size: 15.3 MB (15266557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1370aca8675bcd0ffc32a349297c2d8b6bd8deaf283b5de7a041865ebf38b3`  
		Last Modified: Wed, 21 Sep 2022 00:41:41 GMT  
		Size: 195.4 MB (195388901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
