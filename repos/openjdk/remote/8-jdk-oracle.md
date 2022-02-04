## `openjdk:8-jdk-oracle`

```console
$ docker pull openjdk@sha256:645ee8dd5a1a901482b328c3ef0ad3aebbf9eee71fcead821f12a89d4619f560
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:8-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:d48dde81c26430604881ff1d497ab7b5cc22273ed4505b1027c1b4b757cc79d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161579602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b907bf40ea08338d847c290a8e8c89637fd8b9b204b19bcf99b367fd83acdb8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 05:30:31 GMT
ADD file:17957b69b27e30b1d860c0919546da181b5e126b4aca4e1935ab44fd1832578e in / 
# Fri, 04 Feb 2022 05:30:31 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 06:31:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 04 Feb 2022 06:35:48 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Fri, 04 Feb 2022 06:35:48 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Feb 2022 06:35:48 GMT
ENV LANG=C.UTF-8
# Fri, 04 Feb 2022 06:35:49 GMT
ENV JAVA_VERSION=8u322
# Fri, 04 Feb 2022 06:37:09 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:f431a76c5f59c48efd4a4076677acaae2b540a7562de00075162ef8a340fd69b`  
		Last Modified: Fri, 04 Feb 2022 05:31:30 GMT  
		Size: 42.1 MB (42102405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0509e57e85d3b85eac03c20f8f88d1cb2481d6122bdae0020851f7022e3b31`  
		Last Modified: Fri, 04 Feb 2022 08:22:45 GMT  
		Size: 13.5 MB (13513973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5786d3b61fac424e4ab36e59163ceee32e41d7f58c142485a72ccf268908ca8`  
		Last Modified: Fri, 04 Feb 2022 08:26:28 GMT  
		Size: 106.0 MB (105963224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7611d7dcf4881640fd5e206d21695e0e2a8661b0735c6f289486225af6232a3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.3 MB (161284220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76aac169512d25fb2dd301f26b33d3bff064b40b8cf4a92ef6ccfaf83c84923b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 04:13:53 GMT
ADD file:22ac13d97f9f75668fec05f2cf9d182e5edcf2822b08ef38929b0bb8d61f5edb in / 
# Fri, 04 Feb 2022 04:13:54 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 05:34:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 04 Feb 2022 05:41:32 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Fri, 04 Feb 2022 05:41:33 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Feb 2022 05:41:34 GMT
ENV LANG=C.UTF-8
# Fri, 04 Feb 2022 05:41:35 GMT
ENV JAVA_VERSION=8u322
# Fri, 04 Feb 2022 05:41:45 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:200ed4b56d545919e183ba8dfa2493452065262be1759dd78c3de721a71882cb`  
		Last Modified: Fri, 04 Feb 2022 04:14:59 GMT  
		Size: 42.0 MB (42011648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4545cbf19e4d384cf8f28f10cdb2cb3e0cfb6a09f47542c1c092358c7fd1b5`  
		Last Modified: Fri, 04 Feb 2022 05:50:37 GMT  
		Size: 14.3 MB (14290526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b6a3b60ea84203db735712c241c84c51cf2de612f0f9fa2dfe35e9a59a53d9`  
		Last Modified: Fri, 04 Feb 2022 05:55:15 GMT  
		Size: 105.0 MB (104982046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
