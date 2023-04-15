## `openjdk:21-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:7ee7d0a5e139611d2daf44a3121292c40fd985ef2530812f26ce18f9f037fa46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:80ce333f40fd9d777f1e25c637cbde02799a9c65276d420ab8ffa5daa39446dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266154819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79fa98bf2a7ca61546e838cec6950dd253ff7ef15dcc2371cee70d48a805a81c`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 Mar 2023 22:29:01 GMT
ADD file:a14b5a8b8b6993aeee5ac6052fdf283560d65365e5bcf133ab21c4756439384a in / 
# Fri, 31 Mar 2023 22:29:01 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 23:12:41 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 31 Mar 2023 23:12:42 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 31 Mar 2023 23:12:42 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 31 Mar 2023 23:12:42 GMT
ENV LANG=en_US.UTF-8
# Sat, 15 Apr 2023 00:30:17 GMT
ENV JAVA_VERSION=21-ea+18
# Sat, 15 Apr 2023 00:30:39 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='1c6d7b740ced597243d8c05f823f81728a618c73ffa4cbe28a6d3e2eba02ce00'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='b0009295c1ef02c743fc272b654b11bd506714e8efedc881295a1de74e87d8a8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 15 Apr 2023 00:30:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e83e8f2e82cc31391cd0cb4f5ba574ba5eb9708fc0f5dcc34fef53b03ef28f31`  
		Last Modified: Fri, 31 Mar 2023 22:30:40 GMT  
		Size: 50.5 MB (50496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7475b337670740c8f411f4efcbf2d4308101210ec581e69836860ffcd789ca`  
		Last Modified: Fri, 31 Mar 2023 23:14:05 GMT  
		Size: 14.2 MB (14240731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0679c71abcc0d2b08a353a87473cf57c740938455ca8cedb37c72c814630a3`  
		Last Modified: Sat, 15 Apr 2023 00:33:03 GMT  
		Size: 201.4 MB (201418059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:12971d665b3bc4bd65ded21c30fa30d4de0a28b58bfa77beac02316a497cc25b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.1 MB (266066320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5212f0290af82f1bca3fa661803b44c861885bf40553fbe50174fbbdaa1484ae`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 Mar 2023 21:40:35 GMT
ADD file:4fe62bcdc8f181de8e01e791570bbb89f29712a9aef0b329febd817f4fef8887 in / 
# Fri, 31 Mar 2023 21:40:36 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 22:08:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 31 Mar 2023 22:08:06 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 31 Mar 2023 22:08:06 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 31 Mar 2023 22:08:06 GMT
ENV LANG=en_US.UTF-8
# Sat, 15 Apr 2023 00:55:45 GMT
ENV JAVA_VERSION=21-ea+18
# Sat, 15 Apr 2023 00:55:57 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='1c6d7b740ced597243d8c05f823f81728a618c73ffa4cbe28a6d3e2eba02ce00'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='b0009295c1ef02c743fc272b654b11bd506714e8efedc881295a1de74e87d8a8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 15 Apr 2023 00:55:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a138fe98397d054834e86c902a0b929bd7cf0261ac671e779f872176569996ab`  
		Last Modified: Fri, 31 Mar 2023 21:42:01 GMT  
		Size: 51.1 MB (51054832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61213d9405aef8db0237e9542508819c698c4d8293ccbd8799a36206032fdd7c`  
		Last Modified: Fri, 31 Mar 2023 22:09:32 GMT  
		Size: 15.2 MB (15237973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d5eb9aeefffc5931caff1231d466d1daca3019259b5fcf57ce5dd7ccf059e1`  
		Last Modified: Sat, 15 Apr 2023 00:58:12 GMT  
		Size: 199.8 MB (199773515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
