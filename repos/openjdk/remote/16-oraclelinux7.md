## `openjdk:16-oraclelinux7`

```console
$ docker pull openjdk@sha256:c7fff4f9b4a73dfd9147fac99696cd0f664735bb081e27c5b42e80f32ae64743
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:6569596c6e64c64cfa89ecd7a20d01d5363e99ea01ddf7b0bb38783889d1b96c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.5 MB (248476356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f79538d65a4b010264184791be9681a9e3f9cc71fa5c5c57c3792bac86338076`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 12 Feb 2021 00:53:29 GMT
ADD file:361f165903526126476b03dd2afac1fff0b334906bb56d024e5aee87b948b0cf in / 
# Fri, 12 Feb 2021 00:53:29 GMT
CMD ["/bin/bash"]
# Fri, 12 Feb 2021 01:11:19 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 12 Feb 2021 01:12:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 12 Feb 2021 01:12:33 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Feb 2021 01:12:33 GMT
ENV LANG=en_US.UTF-8
# Fri, 12 Feb 2021 01:12:34 GMT
ENV JAVA_VERSION=16
# Fri, 12 Feb 2021 01:13:12 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/35/GPL/openjdk-16_linux-x64_bin.tar.gz'; 			downloadSha256='25f51624a17545a769e97ded5d51075ab31f9a52de925f7292cff951becf8fd2'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/35/GPL/openjdk-16_linux-aarch64_bin.tar.gz'; 			downloadSha256='5afe8561d1c6f777bf0f70bf5d994187ff607b8c4c6ff1194f849a0bb933d805'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 12 Feb 2021 01:13:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a61503a3b32ea964eb926d54dcfe6cd7e21f4e0cca1b1373df21cf904388c445`  
		Last Modified: Fri, 12 Feb 2021 00:54:42 GMT  
		Size: 48.3 MB (48263629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2d02ff646cdda3eb210d43b22353e431d4fa3a204470452ad0a0508cdbf87d`  
		Last Modified: Fri, 12 Feb 2021 01:18:03 GMT  
		Size: 15.4 MB (15437000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ea3eafae0d2f997a653baff55301bdbbc612cd3181ca437d9c00bb2e0f5364`  
		Last Modified: Fri, 12 Feb 2021 01:18:58 GMT  
		Size: 184.8 MB (184775727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:61e0ec12f70eeeb19bd7c8cfd25a63b16118dd65b391a99eca87a56fd29c8ca5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.5 MB (244466068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5be96288f373698c1ec10a158555685be9abd414ad21d07c57ad53b7f4afd11`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 12 Feb 2021 01:00:40 GMT
ADD file:25b64ec41b7ca742c671c416e08a7bee3224e4052650624ef31b5583b1c412df in / 
# Fri, 12 Feb 2021 01:00:41 GMT
CMD ["/bin/bash"]
# Fri, 12 Feb 2021 01:19:33 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 12 Feb 2021 01:20:59 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 12 Feb 2021 01:21:00 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Feb 2021 01:21:00 GMT
ENV LANG=en_US.UTF-8
# Fri, 12 Feb 2021 01:21:01 GMT
ENV JAVA_VERSION=16
# Fri, 12 Feb 2021 01:21:47 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/35/GPL/openjdk-16_linux-x64_bin.tar.gz'; 			downloadSha256='25f51624a17545a769e97ded5d51075ab31f9a52de925f7292cff951becf8fd2'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/35/GPL/openjdk-16_linux-aarch64_bin.tar.gz'; 			downloadSha256='5afe8561d1c6f777bf0f70bf5d994187ff607b8c4c6ff1194f849a0bb933d805'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 12 Feb 2021 01:21:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:da6ef06bd6983a3815530ecb4b6d3bcef6c011f03daa80be12f60c382e0c23e9`  
		Last Modified: Fri, 12 Feb 2021 01:01:42 GMT  
		Size: 48.9 MB (48854102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2cbabffc67d7d6521300614c7fd34cc6a54a4697d98c388898fc060b0f77d3`  
		Last Modified: Fri, 12 Feb 2021 01:26:00 GMT  
		Size: 16.5 MB (16465019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07258516d2a35f143461cc041e06a0901dcef454ca1200ff094ca464747eba4f`  
		Last Modified: Fri, 12 Feb 2021 01:27:19 GMT  
		Size: 179.1 MB (179146947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
