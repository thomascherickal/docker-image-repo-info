## `openjdk:8-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:a38a7ba7f772f744976bc8f73a075c2fee0e2dc4da3d61488bd3c94081499603
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:8-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:b3e62ae01f43ef1c6aac087f1988d88915fdd880df5e97268171869103de1577
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161583089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2cdf89413bd13f7280bab907e4ece9331808ebadea55b4cb6ff12a783df5e2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 11 Feb 2022 18:20:31 GMT
ADD file:636d5d8575ec6ddd380a3bbf41530219d37249378b4abd151d94842377cc55d9 in / 
# Fri, 11 Feb 2022 18:20:32 GMT
CMD ["/bin/bash"]
# Fri, 11 Feb 2022 19:02:04 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Feb 2022 19:05:58 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Fri, 11 Feb 2022 19:05:58 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 19:05:58 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 19:05:58 GMT
ENV JAVA_VERSION=8u322
# Fri, 11 Feb 2022 19:07:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:010357f4c091049bd23724817a1881f575ff94d35f4c621b4f87b2876049650b`  
		Last Modified: Fri, 11 Feb 2022 18:21:24 GMT  
		Size: 42.1 MB (42105112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1b16b3652a6874ccb11ec011003800c33c1d2f3481ede4da46773eb1415faf`  
		Last Modified: Fri, 11 Feb 2022 19:12:10 GMT  
		Size: 13.5 MB (13514759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863085b5aef25eed6109b58811de3888023e28a5bc33ddac5e710aebc307d895`  
		Last Modified: Fri, 11 Feb 2022 19:17:04 GMT  
		Size: 106.0 MB (105963218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c9b8504c232a9bee2f1852e649c9e8901d4935d3f081e78616d9b4c753d7acb5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.3 MB (161306159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e46287043cbd862a066e23baf49f7c6a452272d7ee5d0accd133e774bc1f7b1c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 11 Feb 2022 18:58:36 GMT
ADD file:8d5a0dcc45ab23c7b507e80b63e5752d94837f490600ce95fb8ba8ed2f7baa2d in / 
# Fri, 11 Feb 2022 18:58:37 GMT
CMD ["/bin/bash"]
# Fri, 11 Feb 2022 19:19:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Feb 2022 19:25:32 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Fri, 11 Feb 2022 19:25:32 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 19:25:33 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 19:25:34 GMT
ENV JAVA_VERSION=8u322
# Fri, 11 Feb 2022 19:26:56 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:ffdd659a9f05cadeed9c2d5cead839f585163662ca7f847a41fd64bb4e503f0c`  
		Last Modified: Fri, 11 Feb 2022 18:59:38 GMT  
		Size: 42.0 MB (42018804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73433a5e38bf6b279d0c685ed5c2c34fcb8e2d6755228a9c6c3f3a2313bef9b`  
		Last Modified: Fri, 11 Feb 2022 19:35:51 GMT  
		Size: 14.3 MB (14305278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549350de349a1c00b18829b811d73d8098fef7aaba88923fffbd321992ee70d8`  
		Last Modified: Fri, 11 Feb 2022 19:41:53 GMT  
		Size: 105.0 MB (104982077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
