## `openjdk:18-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:658825096fca9deec5ee4c239e0a59d2e19cb8b049e2ff347fad13ec0afd6941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:7c24da88a9fd2f149ceba7a7e74c236bf1657b0796d71da0740d02051354e1fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.8 MB (251808547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2545f83eebcd7ec9bd86db2e7198d3e1e910b2ca951efa837379fa3ff4f40b51`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 28 Oct 2021 01:23:11 GMT
ADD file:1ba19f36d1d89d348cc182f0c7feb2c27bcca7bd084032525deaba8822462091 in / 
# Thu, 28 Oct 2021 01:23:11 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 01:45:25 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 28 Oct 2021 01:45:25 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 28 Oct 2021 01:45:25 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:45:25 GMT
ENV LANG=en_US.UTF-8
# Thu, 28 Oct 2021 01:45:26 GMT
ENV JAVA_VERSION=18-ea+20
# Thu, 28 Oct 2021 01:45:36 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='aa609b9f3a4a31b3cb3649a39dabf11476d9c5f1f3b8b9583b2be48e14e3c321'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='a1bfee1fed3794347cfce38d0f4a163b7e90702ceb5fe9256d06664c0daa5726'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 28 Oct 2021 01:45:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a755c2d4aa362701b6bb477a4b1cb2594cb0dca6d0e6839e07b0636fb824c7f7`  
		Last Modified: Thu, 28 Oct 2021 01:24:42 GMT  
		Size: 48.3 MB (48328962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d0464e417ebb82551686797f3772337ca857388f6f2209630af5603196a562`  
		Last Modified: Thu, 28 Oct 2021 01:53:12 GMT  
		Size: 15.4 MB (15399150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37811adfbcc4e17e07aadf9b48181650e2e14b8f78e463c812c0ee1e752aea35`  
		Last Modified: Thu, 28 Oct 2021 01:53:24 GMT  
		Size: 188.1 MB (188080435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:aec1d7386eea2f7cdd51704862d7c7019e0eae31b0a504c17d23f2c0a6877fbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.4 MB (252354439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45de6b1adf65e2d54ad7923f315f9750f4ffabbb048d181fcb9f1a115ae31aff`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 28 Oct 2021 01:44:12 GMT
ADD file:f997c704e003e7bef1e40d457d005aa07a60cb4c37255cc2711119deb3e6df7d in / 
# Thu, 28 Oct 2021 01:44:13 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 02:16:09 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 28 Oct 2021 02:16:10 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 28 Oct 2021 02:16:11 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 02:16:12 GMT
ENV LANG=en_US.UTF-8
# Thu, 28 Oct 2021 02:16:13 GMT
ENV JAVA_VERSION=18-ea+20
# Thu, 28 Oct 2021 02:16:30 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='aa609b9f3a4a31b3cb3649a39dabf11476d9c5f1f3b8b9583b2be48e14e3c321'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='a1bfee1fed3794347cfce38d0f4a163b7e90702ceb5fe9256d06664c0daa5726'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 28 Oct 2021 02:16:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9e1221f69ca9b4fd1daae21b9a20e7225f6ca7d0e34e9e998bc6600de1a3836a`  
		Last Modified: Thu, 28 Oct 2021 01:45:43 GMT  
		Size: 48.9 MB (48905370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b5770e043e6b3a738c83528c0b9c0c9be1c26e18eea50e4a5c270c853ccb2e`  
		Last Modified: Thu, 28 Oct 2021 02:29:48 GMT  
		Size: 16.5 MB (16454087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a51fe55839075ca37a9d01f6af29fe41374029eefa0b1f287299a6922bdd8`  
		Last Modified: Thu, 28 Oct 2021 02:30:05 GMT  
		Size: 187.0 MB (186994982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
