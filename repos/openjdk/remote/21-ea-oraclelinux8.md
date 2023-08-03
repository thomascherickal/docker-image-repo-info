## `openjdk:21-ea-oraclelinux8`

```console
$ docker pull openjdk@sha256:1b2f9b423582aba0dd6c2e0a83814f69147ce393ad020aeb7ae027869424182a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:ad7a7d3aac7bd16f0942ee3bdfc8aa5800688d8bea6aec4403fb3c26bfcb5b54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.9 MB (263855668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d78dcaae7f50e31ee3dc19780d17087c481fa09e173a4c457b31aa207d2023`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 22 Jul 2023 01:20:32 GMT
ADD file:6d43f7bf7c8d8c056e6fcc566ccfa2c1e42be1ef095f94d6780d0ca7d9a02e6e in / 
# Sat, 22 Jul 2023 01:20:32 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:40:55 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:41:26 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Sat, 22 Jul 2023 01:41:26 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Jul 2023 01:41:26 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 01:48:12 GMT
ENV JAVA_VERSION=21-ea+33
# Thu, 03 Aug 2023 01:48:35 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/33/GPL/openjdk-21-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='c834bec462c77e18a4ba980cc761754649ad34ee40697597ec64306918dedb0b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/33/GPL/openjdk-21-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='41295b248c50ffe8bfa522c0fce7492eabfad5d0fad5c439e7918949066f225a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 03 Aug 2023 01:48:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:49bb46380f8cb3491e82d000b27a6eb26b2490291da814ce3363bbf2c8baeb1a`  
		Last Modified: Sat, 22 Jul 2023 01:21:47 GMT  
		Size: 44.9 MB (44915006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938c78e257f8d32905a5685feaf98c164b8091b3f15fb7705c4181bd3998b783`  
		Last Modified: Sat, 22 Jul 2023 01:42:50 GMT  
		Size: 15.0 MB (15009045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32fe1f17ad5aebf9ea849212e00b5009a160f953062a072f0c778e9a6ef7c6c`  
		Last Modified: Thu, 03 Aug 2023 01:55:44 GMT  
		Size: 203.9 MB (203931617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7448f5db6ab7ef6f90985ce2d7a0105e50f2eb17afcdea26b9fbc4ba67245479
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.6 MB (261561228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:783c6d891353929de2f4e7cbf7b399fe33032b76aa1420ea5cf80ef6e86b46f5`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:23:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:23:41 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Sat, 22 Jul 2023 01:23:41 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Jul 2023 01:23:41 GMT
ENV LANG=C.UTF-8
# Sat, 22 Jul 2023 01:23:41 GMT
ENV JAVA_VERSION=21-ea+32
# Sat, 22 Jul 2023 01:23:56 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/32/GPL/openjdk-21-ea+32_linux-x64_bin.tar.gz'; 			downloadSha256='465d289c104ada32ecbfaf3e2f820a7f48ac26f32f3b574bf6d6a6521c567c15'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/32/GPL/openjdk-21-ea+32_linux-aarch64_bin.tar.gz'; 			downloadSha256='49275ab32b5c08efa4b6ec1e8900107fb3acc940ede2dad04328ce591b996a2c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 22 Jul 2023 01:23:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87786d2b4c93ec23e4ce18586fdf1f0c0ea5f810fe7a6ea02a197bf01bc37f7`  
		Last Modified: Sat, 22 Jul 2023 01:24:59 GMT  
		Size: 15.7 MB (15670540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7eeb51a4329e8417c930bd85dfc2f2fe6d49601066e61fe4ff4a6751501da78`  
		Last Modified: Sat, 22 Jul 2023 01:26:03 GMT  
		Size: 202.3 MB (202266933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
