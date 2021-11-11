## `openjdk:18-ea-22-oraclelinux8`

```console
$ docker pull openjdk@sha256:dfd040f9cee32064ec20fe0b94447ae2b49da165556b29691dc0d32ff59734f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-22-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:d91c50b89de0c4a4b5d4e9b528995006453b9867cb0dae41f100f89e851c9a52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.7 MB (243728237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:672ef7efeba8fe2ad1d923268b6836d1ecbff55754c90ed0fbfe47b4c214a6f8`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 03 Nov 2021 22:20:09 GMT
ADD file:ee2c184d933cfe1848f54f94d92f5c14d073160b62ec403259b18392d4ec6e1b in / 
# Wed, 03 Nov 2021 22:20:10 GMT
CMD ["/bin/bash"]
# Wed, 03 Nov 2021 22:37:06 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 03 Nov 2021 22:37:07 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 03 Nov 2021 22:37:07 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Nov 2021 22:37:07 GMT
ENV LANG=C.UTF-8
# Thu, 11 Nov 2021 02:27:47 GMT
ENV JAVA_VERSION=18-ea+22
# Thu, 11 Nov 2021 02:27:58 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/22/GPL/openjdk-18-ea+22_linux-x64_bin.tar.gz'; 			downloadSha256='71124796aac929f184d54cf5b2a3ba3a31c0cef1ba9b5b5e1535ec5a5d482a8b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/22/GPL/openjdk-18-ea+22_linux-aarch64_bin.tar.gz'; 			downloadSha256='714a0b84e6ed39e5442ca0044dab9ebecddeceffc9b78aed8e4d7ba2fbefb8aa'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 11 Nov 2021 02:27:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0a6167eaa66c8f2dc1c8dbed1a335f3d4052409454c9f7fbcd8fc35d8576a7e2`  
		Last Modified: Wed, 03 Nov 2021 22:21:16 GMT  
		Size: 42.0 MB (41968115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a88dabbf57eeb24f57debafeba0a2f7b2f4e4e76d1aa9a3bd27edf0682e0f15`  
		Last Modified: Wed, 03 Nov 2021 22:43:12 GMT  
		Size: 13.5 MB (13491241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2f4b2e287c44dde9d335364634f51085f3bc93889ea6d9112410318239f8b6`  
		Last Modified: Thu, 11 Nov 2021 02:34:37 GMT  
		Size: 188.3 MB (188268881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-22-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:11b7e8dfae5d01e55ca294c2d5607eb85d1fda2675d971f139a85b322dd70494
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.3 MB (243341717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86be6e331ab6258ab137976703775c687d43f1294b886cdd612289966000f05b`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 03 Nov 2021 22:44:10 GMT
ADD file:42d3c96053f453ca6f7155adc565cd822cd2663bd2a3862ccaabb9886c191116 in / 
# Wed, 03 Nov 2021 22:44:11 GMT
CMD ["/bin/bash"]
# Wed, 03 Nov 2021 23:01:19 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 03 Nov 2021 23:01:20 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 03 Nov 2021 23:01:21 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Nov 2021 23:01:22 GMT
ENV LANG=C.UTF-8
# Thu, 11 Nov 2021 03:02:37 GMT
ENV JAVA_VERSION=18-ea+22
# Thu, 11 Nov 2021 03:02:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/22/GPL/openjdk-18-ea+22_linux-x64_bin.tar.gz'; 			downloadSha256='71124796aac929f184d54cf5b2a3ba3a31c0cef1ba9b5b5e1535ec5a5d482a8b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/22/GPL/openjdk-18-ea+22_linux-aarch64_bin.tar.gz'; 			downloadSha256='714a0b84e6ed39e5442ca0044dab9ebecddeceffc9b78aed8e4d7ba2fbefb8aa'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 11 Nov 2021 03:02:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f6fe8bd1b591af20f7f1bf6cabe92846a2b5f1ba33ca5fd165cf03624558cd5c`  
		Last Modified: Wed, 03 Nov 2021 22:45:11 GMT  
		Size: 41.9 MB (41879080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f82d768d0f333fffcb86fe10bab796e393363d92953d26c9435077acb1598e`  
		Last Modified: Wed, 03 Nov 2021 23:12:36 GMT  
		Size: 14.3 MB (14274012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f704b15285cc2a20ad1069c10d198679ffef278b4e0230803a2dbc66d599e2ee`  
		Last Modified: Thu, 11 Nov 2021 03:15:04 GMT  
		Size: 187.2 MB (187188625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
