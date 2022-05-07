## `openjdk:19-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:8923de88e72afef1333f2bef13d73871ae3a418583d48e6e4e53fee220373dd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:ce3f6fc453fb96aece9718d87af53491a7c041201977fea52c9cca136ec8cdd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.3 MB (250311494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bae3ad4be6929525c8d6b46f0dec1c431c4222bfe2a358d1e0b6dc07b5560ae4`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 02 May 2022 20:51:06 GMT
ADD file:b2c3e9f338a70507ba6d9ec21f28c7023f4120a45f234ff9a28188119091c60b in / 
# Mon, 02 May 2022 20:51:06 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 21:07:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 02 May 2022 21:07:47 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Mon, 02 May 2022 21:07:47 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 May 2022 21:07:47 GMT
ENV LANG=C.UTF-8
# Mon, 02 May 2022 21:07:47 GMT
ENV JAVA_VERSION=19-ea+20
# Mon, 02 May 2022 21:07:58 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/20/GPL/openjdk-19-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='e5667a2a1208eb3042dd0c3187dd61d10b435204e4d26e466b8f2c7a5d988ce6'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/20/GPL/openjdk-19-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='a5ff38640a2b5097e460a7dd54544f0cbe19b041262549cd3d1015fc81eec50f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 02 May 2022 21:07:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:121b730bab02bd12143950d97a621f2d2dcf4723433bbadc2777d594c871ee71`  
		Last Modified: Mon, 02 May 2022 20:51:57 GMT  
		Size: 42.1 MB (42114330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b275ba7e0da7889811d55da69069fd42118dd8875faded11d9d21a813afe7b`  
		Last Modified: Mon, 02 May 2022 21:13:42 GMT  
		Size: 13.5 MB (13531997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58f75c5ce7a952b6137c658fc6fbc55d813a4528e85b1f6bf9665a6fefc9aa3`  
		Last Modified: Mon, 02 May 2022 21:13:54 GMT  
		Size: 194.7 MB (194665167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:10bf85d8c48b27df5b6b5cdf42541693ab3c1d3afc7fbd0a9d18f6b22ed17166
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.9 MB (249920400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c1e038eb13274946dea3106c1453830917d1157911280cbbdebdf4cf2c805c5`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 02 May 2022 21:46:34 GMT
ADD file:e59d0ab85f777209561c628874489b9544223a23fed0755bedd408a55452b4af in / 
# Mon, 02 May 2022 21:46:35 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 22:06:20 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 02 May 2022 22:06:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Mon, 02 May 2022 22:06:22 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 May 2022 22:06:23 GMT
ENV LANG=C.UTF-8
# Sat, 07 May 2022 00:46:27 GMT
ENV JAVA_VERSION=19-ea+21
# Sat, 07 May 2022 00:46:41 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='8723353dfc5a3dd34d01b96faddc950c48f450083519a62b287fcb1ef82fc446'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e9719e928c6bfa2ed1e3ed7885bc2ff3751e0a8a6c5dde6808dddbd239cba32'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 07 May 2022 00:46:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2d35f3f87cf615a8684aa1b866b03a7078bce1beea91489effc1e6c03c83124c`  
		Last Modified: Mon, 02 May 2022 21:47:34 GMT  
		Size: 42.0 MB (42016620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e242efb2259690773e11adafa3652b3b5f5ac58742dfba66216c5527ec988`  
		Last Modified: Mon, 02 May 2022 22:17:46 GMT  
		Size: 14.3 MB (14292260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a247b11036a9396dc02dcc5e53df822012cccd7835b9037ca82061c052ecab4c`  
		Last Modified: Sat, 07 May 2022 00:58:52 GMT  
		Size: 193.6 MB (193611520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
