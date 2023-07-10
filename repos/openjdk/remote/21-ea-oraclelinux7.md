## `openjdk:21-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:c3cfddec2c303a4d25866179b224c5dd73ef4bc3bd2516d3d8f91cac6d71da98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:ef613bb2e3bd49b09dcc0fdc3ef40a7c56db33f54c600d28a83cf418d5cc91ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268592528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9074b8922f84e4f773609ead655ad766ee4e84e22803204a41caa4e91c7b77`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:56:49 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 14 Jun 2023 09:57:19 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 14 Jun 2023 09:57:19 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 09:57:19 GMT
ENV LANG=en_US.UTF-8
# Mon, 10 Jul 2023 20:48:30 GMT
ENV JAVA_VERSION=21-ea+30
# Mon, 10 Jul 2023 20:48:40 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='c35a1f2906d502e9f75a975165f4c86e29167ca8cc2d9d25b5351b46d90d4ab7'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='ae690af5ffa639feba3bc04fc804480cdbc40b4099890c9d28dceac8f58f0426'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 10 Jul 2023 20:48:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4714d29e017353e367cfbeb707bad46a96692fceb51533b3749c668baf3b5b8f`  
		Last Modified: Wed, 14 Jun 2023 09:58:27 GMT  
		Size: 14.2 MB (14242764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad69cbf0bfbe61b08a02f391ef2b1dfc964504b3dd8ca05259716bf6318171f0`  
		Last Modified: Mon, 10 Jul 2023 20:55:17 GMT  
		Size: 203.9 MB (203864999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:18b03be5f25c5d7ab21fb78a5686d251c290a4e50c5aa1e096d0e1ec987609bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.5 MB (268505072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bfe7a79a5dd1c303886ecd516dc53db375b16f900622f315cf787c48f464037`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 14 Jun 2023 03:45:43 GMT
ADD file:a9ba9c7acb256e802c7248b56f377a6f0ea08b1b61e11e482516633a13f4d686 in / 
# Wed, 14 Jun 2023 03:45:44 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 04:08:20 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 14 Jun 2023 04:08:50 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 14 Jun 2023 04:08:50 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 04:08:50 GMT
ENV LANG=en_US.UTF-8
# Mon, 10 Jul 2023 21:34:53 GMT
ENV JAVA_VERSION=21-ea+30
# Mon, 10 Jul 2023 21:35:05 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='c35a1f2906d502e9f75a975165f4c86e29167ca8cc2d9d25b5351b46d90d4ab7'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='ae690af5ffa639feba3bc04fc804480cdbc40b4099890c9d28dceac8f58f0426'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 10 Jul 2023 21:35:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:52fd87ed40fcddc3fe63b876d1f94f6edae688637a5cc56983dced68a50c953e`  
		Last Modified: Wed, 14 Jun 2023 03:46:28 GMT  
		Size: 51.1 MB (51052081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aeb39f5d39e6fb51e698f8f5e6416d0689047f9392a9bd3f97f28c4d5d5596`  
		Last Modified: Wed, 14 Jun 2023 04:10:01 GMT  
		Size: 15.2 MB (15238146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210301ac818a311ea8d9f941b04f05ad874dff00a6bb1041f3ae8175dc6a1804`  
		Last Modified: Mon, 10 Jul 2023 21:41:05 GMT  
		Size: 202.2 MB (202214845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
