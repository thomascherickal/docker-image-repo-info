## `openjdk:20-oraclelinux7`

```console
$ docker pull openjdk@sha256:5c3f714c150944622780bb50a6924b48f715405969ad4cb049c05e54d2177a1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:b05535bf6749a85f794a455d9d89a0ad3c39e063a3c2c6b290f4b8b002c1d7e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.3 MB (262281859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:442010117bc57a1c54f25aaddebb389fccdb0f4bebb45244e8a92e800908449f`
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
# Fri, 11 Nov 2022 00:56:05 GMT
ENV JAVA_VERSION=20-ea+23
# Fri, 11 Nov 2022 00:56:16 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='0344aa24310a388514ddbc4a0279a9e28f222ae783ac918860ef8f13cfebabbe'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='57ae94d8d6968fc4b6603eab15361e998664b7bb1707611dfa4ab9542c17fd24'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Nov 2022 00:56:17 GMT
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
	-	`sha256:7987b44c3fa8f3f78ae1d5a763d71d0a69028579c53988bc3f6acd12bea31527`  
		Last Modified: Fri, 11 Nov 2022 01:00:54 GMT  
		Size: 198.2 MB (198235821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b88563304630e9a970217b59eca74aa85f0407a216cb7d5729cc4eb343441a31
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.5 MB (262461481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1d2cb988d4532f406823b9b74bea07ef67b5506db10d80fcabfb4343578bbdc`
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
# Fri, 11 Nov 2022 11:33:46 GMT
ENV JAVA_VERSION=20-ea+23
# Fri, 11 Nov 2022 11:34:03 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='0344aa24310a388514ddbc4a0279a9e28f222ae783ac918860ef8f13cfebabbe'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='57ae94d8d6968fc4b6603eab15361e998664b7bb1707611dfa4ab9542c17fd24'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Nov 2022 11:34:05 GMT
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
	-	`sha256:b93515d609c727d702f08d6cbaf99a4f924b26aa164d31ce7f111b109e9243eb`  
		Last Modified: Fri, 11 Nov 2022 11:38:38 GMT  
		Size: 196.8 MB (196797033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
