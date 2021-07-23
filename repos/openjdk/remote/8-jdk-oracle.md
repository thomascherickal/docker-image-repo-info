## `openjdk:8-jdk-oracle`

```console
$ docker pull openjdk@sha256:fe675cfd9590576d6c2ced2092eb7cb44ef757eacb07ba63d6d324c37c1ee50b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:8-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:d67fd5af7601f5767cb6b9070f11fbd37728b084e482f4adfd85ad65366194d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.5 MB (161450529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b72549befe7607011938e70b77ce6879acf87731737e4d5f5cbfd82f3979b88`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 01:13:10 GMT
ADD file:c047ac1784a3670f52d12ad67cf238654237149dc2c9d7b921cd005c7ec42105 in / 
# Fri, 23 Jul 2021 01:13:11 GMT
CMD ["/bin/bash"]
# Fri, 23 Jul 2021 06:40:31 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 23 Jul 2021 06:44:10 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Fri, 23 Jul 2021 06:44:11 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:44:11 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 06:44:11 GMT
ENV JAVA_VERSION=8u302
# Fri, 23 Jul 2021 06:44:23 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:1da50e1664e1b58d93182fe5af093c642668ec93f67fcd8215b9c1979930b84d`  
		Last Modified: Fri, 23 Jul 2021 01:14:27 GMT  
		Size: 42.2 MB (42178827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c8e5a84542212d0126ce88facd146befb1c731fb4faafb50a7b96ad0568cd9`  
		Last Modified: Fri, 23 Jul 2021 06:49:18 GMT  
		Size: 13.4 MB (13390485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354ac4a83bf4111c921ce43bf058256f7279c409350596ca89554e742bca3272`  
		Last Modified: Fri, 23 Jul 2021 06:54:16 GMT  
		Size: 105.9 MB (105881217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:8538392b67af803a00cb84c589375d0b5b018f5df877fb0282851d069a8c107f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.1 MB (161109719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7924aae498d25aeecf572b808eb69cd576f2af87446feafa71e1f597b3032509`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 00:50:01 GMT
ADD file:2b2b9653730f3bb9d3a6327d4b9a6b425279decd90b84755c033b95536ebe027 in / 
# Fri, 23 Jul 2021 00:50:02 GMT
CMD ["/bin/bash"]
# Fri, 23 Jul 2021 04:34:01 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 23 Jul 2021 04:37:39 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Fri, 23 Jul 2021 04:37:39 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 04:37:40 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 04:37:40 GMT
ENV JAVA_VERSION=8u302
# Fri, 23 Jul 2021 04:37:48 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:a21bf021f71862240d392ffdd7f376294fa46f2729f1771f269c1a888d0aab25`  
		Last Modified: Fri, 23 Jul 2021 00:51:19 GMT  
		Size: 42.0 MB (42040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20d17a0583d5448fece8a45dc16fcd83266885f5eabbeaa44c9bcc8738ed0fa`  
		Last Modified: Fri, 23 Jul 2021 04:45:32 GMT  
		Size: 14.2 MB (14170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708b562666b12e2ac4b624b94ada5dfe3397259b3bd22baa61c8f6be6666febc`  
		Last Modified: Fri, 23 Jul 2021 04:51:29 GMT  
		Size: 104.9 MB (104898049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
