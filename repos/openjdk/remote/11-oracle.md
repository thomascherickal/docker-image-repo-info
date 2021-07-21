## `openjdk:11-oracle`

```console
$ docker pull openjdk@sha256:bf9902827aaa4e00faecfc20278ce2879bf7ef06fa8654d62220e6b590938d08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:11-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:b581bb6c7bf15cc5c45b9d9a06b3b991945666f67562033a976c31b1d44e24b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.6 MB (258585329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0777e448512c2b097906fe0c81d56396291ebb4f69c15d6e571f47ac03ce7335`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jul 2021 20:20:57 GMT
ADD file:c830de449b9ecd90e02f56d99e8326701da17970fa314bd7b060fd9a7cf7ac77 in / 
# Mon, 12 Jul 2021 20:20:58 GMT
CMD ["/bin/bash"]
# Mon, 12 Jul 2021 23:33:03 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 12 Jul 2021 23:36:36 GMT
ENV JAVA_HOME=/usr/java/openjdk-11
# Mon, 12 Jul 2021 23:36:36 GMT
ENV PATH=/usr/java/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 12 Jul 2021 23:36:37 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 18:23:22 GMT
ENV JAVA_VERSION=11.0.12
# Wed, 21 Jul 2021 18:23:38 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Jul 2021 18:23:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c828c776e142cb23ad61c84403bb42deaa97efeda5e2b600df46f7dbd38ec681`  
		Last Modified: Mon, 12 Jul 2021 20:22:25 GMT  
		Size: 42.2 MB (42179737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8846dac42cae4499c0917b5bd5e81c0e6d6fcc5326d50972b3faed7ccdf688b8`  
		Last Modified: Mon, 12 Jul 2021 23:41:34 GMT  
		Size: 13.4 MB (13392657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1928280b69aaba5b30d1f143f7227143c48f2d265bfd662d3caee450549f13`  
		Last Modified: Wed, 21 Jul 2021 18:31:42 GMT  
		Size: 203.0 MB (203012935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7a3c8de43cb24ba1411315ec7486b08b52f5db99484bd57ab11143a3ae4bfc86
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.9 MB (256853888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46acf85b2c753b140602744f96a605c63b8b9d0a8cda4c3c3229ded57f471cfb`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jul 2021 20:40:32 GMT
ADD file:a184ed870dc7a85028f7ba3bd0cf3820d6f1b94ac4cea1ac94ca48c786901041 in / 
# Mon, 12 Jul 2021 20:40:33 GMT
CMD ["/bin/bash"]
# Mon, 12 Jul 2021 21:03:05 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 12 Jul 2021 21:05:54 GMT
ENV JAVA_HOME=/usr/java/openjdk-11
# Mon, 12 Jul 2021 21:05:54 GMT
ENV PATH=/usr/java/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 12 Jul 2021 21:05:54 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 18:45:07 GMT
ENV JAVA_VERSION=11.0.12
# Wed, 21 Jul 2021 18:45:22 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Jul 2021 18:45:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6186b25cabd91cbdd2c6bf65b0c5ef261f52719e7c6c4d6252e7082b7a51b42e`  
		Last Modified: Mon, 12 Jul 2021 20:41:48 GMT  
		Size: 42.1 MB (42072715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8304774b066b61c2ae3dc6de204cb3d384a726b9376d301afc654577b50a9c0`  
		Last Modified: Mon, 12 Jul 2021 21:15:51 GMT  
		Size: 14.2 MB (14170180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1eaf21aec10a8c3db3ddf273a181193e2abf83a738f2569b2870352f644d32`  
		Last Modified: Wed, 21 Jul 2021 18:59:08 GMT  
		Size: 200.6 MB (200610993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
