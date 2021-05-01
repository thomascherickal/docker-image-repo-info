## `openjdk:17-ea-20-oracle`

```console
$ docker pull openjdk@sha256:52f677d789b31b6b81d746716fa48d7ce654161aff62e45c72d89183ee0dc7c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-ea-20-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:63a06e2c6b4016567f2bb229cc24beb514a8bff8f2383159fae582032471fb3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241338543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebf093474ff2b163f627fbc8371c8c66292d8af7d3aab8fff03c88f69aed6d90`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 17 Apr 2021 01:21:29 GMT
ADD file:9c532b9932419aab70115bea018132ac9096e9eebb25f230bda99cb66245fab2 in / 
# Sat, 17 Apr 2021 01:21:29 GMT
CMD ["/bin/bash"]
# Sat, 17 Apr 2021 01:38:22 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 17 Apr 2021 01:38:22 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Sat, 17 Apr 2021 01:38:22 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 17 Apr 2021 01:38:22 GMT
ENV LANG=C.UTF-8
# Sat, 01 May 2021 03:39:04 GMT
ENV JAVA_VERSION=17-ea+20
# Sat, 01 May 2021 03:39:15 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='2de5c546c3e38f36676c7e22dd040e5b540fc258f72194e7ae17af3f2bf7f0b5'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='9e376a3f2c9a3dc5394fc2f3da480f72b9103c3b71d39d041dc6b08bb65e5724'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 01 May 2021 03:39:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9509c6b41a37fbf5dbb93aedded1aff0dc6ed45ab2d334440e10a5c8d112531c`  
		Last Modified: Sat, 17 Apr 2021 01:22:39 GMT  
		Size: 42.1 MB (42063762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0005db77786a07e4e5d56adc224c9dc85320b46354f9110eb174ce7df9df04`  
		Last Modified: Sat, 17 Apr 2021 01:43:53 GMT  
		Size: 13.3 MB (13272982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5f496cc317d0c1629ec3441d92034406388aa49e7ac7f629c6a732c02c919`  
		Last Modified: Sat, 01 May 2021 03:44:27 GMT  
		Size: 186.0 MB (186001799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-20-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:af872774497ca45b6e65f04a10c102363e8f4acd1729f6a954996f0da16766ac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.1 MB (238112539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eee0ba3db3580563f324b67283d850706562e4850f7e9cd472bc97788cc15248`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 17 Apr 2021 00:43:47 GMT
ADD file:2afad2b68d4889be2ef517aea246957975145f8ad99a3e9e6a01baf79f67d5e2 in / 
# Sat, 17 Apr 2021 00:43:51 GMT
CMD ["/bin/bash"]
# Sat, 17 Apr 2021 01:01:42 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 17 Apr 2021 01:01:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Sat, 17 Apr 2021 01:01:44 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 17 Apr 2021 01:01:45 GMT
ENV LANG=C.UTF-8
# Sat, 01 May 2021 01:17:50 GMT
ENV JAVA_VERSION=17-ea+20
# Sat, 01 May 2021 01:18:46 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='2de5c546c3e38f36676c7e22dd040e5b540fc258f72194e7ae17af3f2bf7f0b5'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='9e376a3f2c9a3dc5394fc2f3da480f72b9103c3b71d39d041dc6b08bb65e5724'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 01 May 2021 01:18:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4b26d50a92155f32c82c580c6abd80083d4fff230a35ef647094df38f4475f9f`  
		Last Modified: Sat, 17 Apr 2021 00:45:12 GMT  
		Size: 42.0 MB (41996718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc97fa408166ea1b3901653a092a35a895b8718e00810a9bf87dd8f1d0430f3`  
		Last Modified: Sat, 17 Apr 2021 01:07:39 GMT  
		Size: 14.0 MB (14034435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5622382afc27f54718bfb4da11613ae12eee4e86b910c18045a465a61e39cb1f`  
		Last Modified: Sat, 01 May 2021 01:26:32 GMT  
		Size: 182.1 MB (182081386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
