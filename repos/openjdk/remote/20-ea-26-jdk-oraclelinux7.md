## `openjdk:20-ea-26-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:da77dd2c72a5147ff7251a55d49ad62be325e898b590f62bbf9ca358ba2e5bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-26-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:4e71545361675ff739a92c5eda0030d1ab47f433d63ebedd7b9a36324811839f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.0 MB (261995900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:790c29adbcf83bcff86ef4363a6548d826c78a693100ff4dc7420bbf03e7c9c4`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 29 Nov 2022 19:21:24 GMT
ADD file:ec2c8d4fc7614a3584827f15c6278d01c6d7f42892747f20aeccfa2feb526412 in / 
# Tue, 29 Nov 2022 19:21:25 GMT
CMD ["/bin/bash"]
# Tue, 29 Nov 2022 19:44:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 29 Nov 2022 19:44:29 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Tue, 29 Nov 2022 19:44:29 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Nov 2022 19:44:30 GMT
ENV LANG=en_US.UTF-8
# Fri, 02 Dec 2022 00:21:37 GMT
ENV JAVA_VERSION=20-ea+26
# Fri, 02 Dec 2022 00:21:48 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='70075a76ed683898d8d71852394c88ab73d8665b15accfafa85dac3be5fbf87e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='041c2b0e7b68e58376d8b03db365434ceecd65671de20af28e6c32f47ccde94a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 02 Dec 2022 00:21:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d96bccd7291ff1dc9e55f40b596e14900d110382763aa46814bc43ac1b40f57c`  
		Last Modified: Tue, 29 Nov 2022 19:23:17 GMT  
		Size: 49.8 MB (49828163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dc1504ba6d49eee445e92e7d82d816810257ac694a462bb310e1d2bf178fd8`  
		Last Modified: Tue, 29 Nov 2022 19:48:44 GMT  
		Size: 14.2 MB (14217773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2c4cce83a120d2126ea34acad3d1f486521b1fa35cd37ce66ddb94b73fddd2`  
		Last Modified: Fri, 02 Dec 2022 00:26:13 GMT  
		Size: 197.9 MB (197949964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-26-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:67b79c89666c85f1dbeeabb75b645db8518328b9faeb9b9f46e3c2361675b9d4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.2 MB (262167744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ecd0dd1c67811e75fe82655782730a8654a85a672dbecc89ca9f65d20914d6b`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 29 Nov 2022 19:48:43 GMT
ADD file:5019a53be0205e5de5a1e1425dc3a4e8d6300733ab4bb1cdc29a6dbfc6a6a12c in / 
# Tue, 29 Nov 2022 19:48:44 GMT
CMD ["/bin/bash"]
# Tue, 29 Nov 2022 20:06:51 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 29 Nov 2022 20:06:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Tue, 29 Nov 2022 20:06:52 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Nov 2022 20:06:52 GMT
ENV LANG=en_US.UTF-8
# Thu, 01 Dec 2022 23:43:34 GMT
ENV JAVA_VERSION=20-ea+26
# Thu, 01 Dec 2022 23:43:45 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='70075a76ed683898d8d71852394c88ab73d8665b15accfafa85dac3be5fbf87e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='041c2b0e7b68e58376d8b03db365434ceecd65671de20af28e6c32f47ccde94a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 01 Dec 2022 23:43:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:32a97da7a0b03315fbde64fde482eae59f8581d380cfa0e24b35ffd3ad1d1bf2`  
		Last Modified: Tue, 29 Nov 2022 19:50:24 GMT  
		Size: 50.4 MB (50399247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7565e5cd26c7105898fa9f6b8389575df84b097aec6966840da625b7e2a3c7e9`  
		Last Modified: Tue, 29 Nov 2022 20:10:57 GMT  
		Size: 15.3 MB (15268420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79343e777c980dd1a11c8f0b4b5cc84c0dcc0c6ef8051deb7c278b0ae3b9275d`  
		Last Modified: Thu, 01 Dec 2022 23:48:18 GMT  
		Size: 196.5 MB (196500077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
