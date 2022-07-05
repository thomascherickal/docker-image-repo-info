## `openjdk:8-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:4098bc67258c38ecaf21efb95c511a7b85f4410a4ad75fcb259b79ae737951a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:8-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:c926b259bb6ba40891202726a3f1ebd7b57291fafdd00a34e893070e6394458e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.8 MB (168844783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb01627b0ef214f10504cc39a72dc515f0e1d61c90d54edcd15fab11ee2fc741`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:58 GMT
ADD file:50fb7d83a9d57e5a0a6af5e5daf27e464ae8a28c196ce6bad6c254dfc1774cdd in / 
# Tue, 05 Jul 2022 22:20:58 GMT
CMD ["/bin/bash"]
# Tue, 05 Jul 2022 22:50:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 05 Jul 2022 22:53:24 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Tue, 05 Jul 2022 22:53:24 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Jul 2022 22:53:24 GMT
ENV LANG=en_US.UTF-8
# Tue, 05 Jul 2022 22:53:24 GMT
ENV JAVA_VERSION=8u332
# Tue, 05 Jul 2022 22:53:31 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_linux_8u332b09.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_aarch64_linux_8u332b09.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:66fb3478003364657ac7751c40e41a135e02975f9459f652b1df23e3896b5fac`  
		Last Modified: Tue, 05 Jul 2022 22:22:18 GMT  
		Size: 48.8 MB (48762895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8f0f1eb3582fe120c104ded4086894e324ef46a631953f821f879e3e7a6a26`  
		Last Modified: Tue, 05 Jul 2022 22:58:49 GMT  
		Size: 14.2 MB (14245779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3642108a99b506dff6f9566da495371d9e102e6de166ccf2e1708910c93818`  
		Last Modified: Tue, 05 Jul 2022 23:06:19 GMT  
		Size: 105.8 MB (105836109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:d10c72e9682a7777af43608afb45a2f10d3a56e1b22cda6c8707cee59e3a7d93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169417520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d78d61ca0e7bdf3b4c0aeab2ca484838482ab661087f088d9001c0e4a9cfe4c9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:37 GMT
ADD file:6d5eeb6c0921661dff8e0b6a89c3272aa52f72b5926d62ae482a85c8ef6458a3 in / 
# Tue, 05 Jul 2022 22:43:38 GMT
CMD ["/bin/bash"]
# Tue, 05 Jul 2022 23:05:04 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 05 Jul 2022 23:11:28 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Tue, 05 Jul 2022 23:11:29 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Jul 2022 23:11:30 GMT
ENV LANG=en_US.UTF-8
# Tue, 05 Jul 2022 23:11:31 GMT
ENV JAVA_VERSION=8u332
# Tue, 05 Jul 2022 23:11:43 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_linux_8u332b09.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_aarch64_linux_8u332b09.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:456ca0cbf3e695c518e5d5c4cb5ff9f99bb999a28b5ec7da3b4ca48d3cf80e6b`  
		Last Modified: Tue, 05 Jul 2022 22:45:10 GMT  
		Size: 49.3 MB (49342729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7981fd8b8b8e53f7977497096fa392e1d14f1e3dd10684ac47d3fa4688b887e7`  
		Last Modified: Tue, 05 Jul 2022 23:21:54 GMT  
		Size: 15.3 MB (15264543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3525bbf40bd1ac74f5e4849adc9182c1cca7ffa914a2a23fc410928224f19e`  
		Last Modified: Tue, 05 Jul 2022 23:30:31 GMT  
		Size: 104.8 MB (104810248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
