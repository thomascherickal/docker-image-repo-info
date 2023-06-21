## `openjdk:22-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:86cc7078b7292035d3ff19030819dcbbf08c134929a998b1946cc6586951e219
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:e702c9c92492b1ac472f10c5e278e1a91024f14c406765b3e32d11fd4b2372aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.3 MB (269332235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb0922e5e3627bca57e4e87c000f868397403c9de7d58e79a3e02be2db1a793d`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:56:49 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 14 Jun 2023 09:56:49 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Wed, 14 Jun 2023 09:56:49 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 09:56:49 GMT
ENV LANG=en_US.UTF-8
# Wed, 21 Jun 2023 01:12:16 GMT
ENV JAVA_VERSION=22-ea+2
# Wed, 21 Jun 2023 01:12:28 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/2/GPL/openjdk-22-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='d759c4f3b3cf116701356fb6276cbe5cebac2ff8fbc88e7ca0c10db5c659bf0b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/2/GPL/openjdk-22-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='b60aa1790dc7fa69e983498162b3e0cd883ddc0d89319529cf9dd381b3b04ded'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Jun 2023 01:12:29 GMT
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
	-	`sha256:254eed5e5a4c4faf29be9be7449d70ccdd9aff50f6b60bee451a90448d410107`  
		Last Modified: Wed, 21 Jun 2023 01:17:52 GMT  
		Size: 204.6 MB (204604706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:aa4caa44004996f20e6038545d5b40545cc264b2331a3bb37e5da2616b909ea9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.2 MB (269219902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f551335b45ff03ef528fdd093ae9a62ce85aabb630ee5ef2a1e6ef4e5f045ab9`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 14 Jun 2023 03:45:43 GMT
ADD file:a9ba9c7acb256e802c7248b56f377a6f0ea08b1b61e11e482516633a13f4d686 in / 
# Wed, 14 Jun 2023 03:45:44 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 04:08:20 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 14 Jun 2023 04:08:20 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Wed, 14 Jun 2023 04:08:20 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 04:08:20 GMT
ENV LANG=en_US.UTF-8
# Wed, 21 Jun 2023 01:13:16 GMT
ENV JAVA_VERSION=22-ea+2
# Wed, 21 Jun 2023 01:13:38 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/2/GPL/openjdk-22-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='d759c4f3b3cf116701356fb6276cbe5cebac2ff8fbc88e7ca0c10db5c659bf0b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/2/GPL/openjdk-22-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='b60aa1790dc7fa69e983498162b3e0cd883ddc0d89319529cf9dd381b3b04ded'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Jun 2023 01:13:40 GMT
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
	-	`sha256:cbb03b8e10373f5410ed73ec1990cbf95a3bb875048a824df86b9c3ba97c4e64`  
		Last Modified: Wed, 21 Jun 2023 01:18:39 GMT  
		Size: 202.9 MB (202929675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
