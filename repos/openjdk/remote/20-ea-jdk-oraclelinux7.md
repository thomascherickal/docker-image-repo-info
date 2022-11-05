## `openjdk:20-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:7f993646164d5d4f360e64b7fa0d2849812b97edb2d457dd8967c96290740917
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:458d22aafa63f442c5b1cf4f5937b8f573cd6e997363ea85f4c96dad844fa02c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.3 MB (262319144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3fd7b751d458db92700d48d58b61a89c237aef62fd308bbeb07b1ada9bfa68`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:35 GMT
ADD file:aaaadfdf901c2df5f641e6c43b10817fcbd0caca73acb7672608f43ba71cefeb in / 
# Fri, 04 Nov 2022 23:33:36 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:20:17 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Sat, 05 Nov 2022 02:20:17 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Sat, 05 Nov 2022 02:20:17 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 02:20:17 GMT
ENV LANG=en_US.UTF-8
# Sat, 05 Nov 2022 02:20:18 GMT
ENV JAVA_VERSION=20-ea+21
# Sat, 05 Nov 2022 02:20:29 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/21/GPL/openjdk-20-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='7cb7563541c5a384bcdac868744a5faeea2fa8bd68f5e0f2ee03ffa27d1f9d56'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/21/GPL/openjdk-20-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='f63aac8e75f05ed5212a7365be1007c6995c7f10d6f9308f8894634455d9a0f4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 05 Nov 2022 02:20:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9a0b9cd2dfe62ff7a933afe41891425abf01b0aaed70cedb028f03392d60037f`  
		Last Modified: Fri, 04 Nov 2022 23:35:26 GMT  
		Size: 49.8 MB (49827924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd91916b9b5718027cc164239330e952a98aeb093ce9bd81860aa1729904850`  
		Last Modified: Sat, 05 Nov 2022 02:24:18 GMT  
		Size: 14.2 MB (14218114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1332df96b91bbdef8473aed03f71ffa5fa411cbae343befe5dfd1d66aa16a607`  
		Last Modified: Sat, 05 Nov 2022 02:24:31 GMT  
		Size: 198.3 MB (198273106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:330e74c31342a3b109824f054093a10eb4dca4ddefc09bd460c7f1eff4e2413b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.5 MB (262515158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67fe020578658ba89354e564062b9026913d52d53bda9c7c10fd872fdaddb7e4`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Nov 2022 22:50:27 GMT
ADD file:4d172a457b1d27e8913a5e05a18d79d4b651e2d8677c9391e5d838f8b88ecaf7 in / 
# Fri, 04 Nov 2022 22:50:28 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 00:50:12 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Sat, 05 Nov 2022 00:50:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Sat, 05 Nov 2022 00:50:12 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 00:50:12 GMT
ENV LANG=en_US.UTF-8
# Sat, 05 Nov 2022 00:50:13 GMT
ENV JAVA_VERSION=20-ea+21
# Sat, 05 Nov 2022 00:50:24 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/21/GPL/openjdk-20-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='7cb7563541c5a384bcdac868744a5faeea2fa8bd68f5e0f2ee03ffa27d1f9d56'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/21/GPL/openjdk-20-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='f63aac8e75f05ed5212a7365be1007c6995c7f10d6f9308f8894634455d9a0f4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 05 Nov 2022 00:50:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bb54b8cf6e14ad1a2ea509cf62cacf70a75fe1fc21dba31199165b9534e1b8c1`  
		Last Modified: Fri, 04 Nov 2022 22:52:11 GMT  
		Size: 50.4 MB (50401543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25e3b537f11ad791c5f6c0140d98f0ff4716add37dcc3762f87c091b8d79048`  
		Last Modified: Sat, 05 Nov 2022 00:54:35 GMT  
		Size: 15.3 MB (15262905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9ec6ad8350839d677809459f05b847220c428a13d15b46e17d4cd8d5b97ad3`  
		Last Modified: Sat, 05 Nov 2022 00:54:46 GMT  
		Size: 196.9 MB (196850710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
