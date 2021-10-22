## `openjdk:8-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:58ddb6ddb94f10bcb112546f95057b4ca34e602a25c21518bdeafb81844857d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:8-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:1210db233e63fbc67ac610384715ed682bd7bfa28f5382346d6477b46f91399d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169527548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7c8c37c51ce89b4c78e76ad88c4bff0d0b0a923a4fc7e15cd318a2ebe53293b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Oct 2021 18:30:19 GMT
ADD file:a6def617e1c0cf7def2d3ce3c79073621ed8efb37deed65fb49e7fc0a6d8ea37 in / 
# Wed, 13 Oct 2021 18:30:20 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 18:48:31 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 13 Oct 2021 18:52:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Wed, 13 Oct 2021 18:52:21 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 18:52:21 GMT
ENV LANG=en_US.UTF-8
# Thu, 21 Oct 2021 23:46:37 GMT
ENV JAVA_VERSION=8u312
# Thu, 21 Oct 2021 23:46:50 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:e0ada0403966475cc22d4e65b5fd1bde8aac848d542317ef0154b8961c767d23`  
		Last Modified: Wed, 13 Oct 2021 18:31:57 GMT  
		Size: 48.2 MB (48235779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ebd61f33542411694b578674a48c8a09f401b78b67f813518bff7eb70dbbb`  
		Last Modified: Wed, 13 Oct 2021 18:57:37 GMT  
		Size: 15.4 MB (15397943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298d39344bbe3088d1d68b07af551e8e5ac6f5177b3081e76206cff3e2466959`  
		Last Modified: Fri, 22 Oct 2021 00:02:55 GMT  
		Size: 105.9 MB (105893826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:adf725f6c17bf47ae47fa46321b85a1e2c69cd56cfc81a68ca52f1e1e425c001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170165883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64b35271116bc57519b626e6fc74e5dc9f933316c6bdf35309522ed2e2e2fb6a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 14 Oct 2021 03:43:46 GMT
ADD file:fca1474953cf608c9b2613787e7e7b859d458af91405a97dbd4ee57c63565185 in / 
# Thu, 14 Oct 2021 03:43:47 GMT
CMD ["/bin/bash"]
# Thu, 14 Oct 2021 05:43:29 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 14 Oct 2021 05:49:29 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Thu, 14 Oct 2021 05:49:30 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Oct 2021 05:49:31 GMT
ENV LANG=en_US.UTF-8
# Thu, 14 Oct 2021 05:49:32 GMT
ENV JAVA_VERSION=8u302
# Thu, 14 Oct 2021 05:50:12 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:1322b24b1fa49fc9b6d0dad59ae623077ce5c89f6aca858053f6d7e45222e954`  
		Last Modified: Thu, 14 Oct 2021 03:45:17 GMT  
		Size: 48.8 MB (48820013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dfa211810869c7e6ae1a8fdb375623b16dc354d9e55dd50190c994ba3b3263`  
		Last Modified: Thu, 14 Oct 2021 05:58:58 GMT  
		Size: 16.4 MB (16447841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e07234ab7a41e611627872ead21051d5b6d5b0505a2b8bbbf2c3a111216567`  
		Last Modified: Thu, 14 Oct 2021 06:06:20 GMT  
		Size: 104.9 MB (104898029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
