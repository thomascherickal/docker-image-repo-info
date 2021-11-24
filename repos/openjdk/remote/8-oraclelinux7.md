## `openjdk:8-oraclelinux7`

```console
$ docker pull openjdk@sha256:4ced8f7c75f751b3e79c9bd07085c6ba88a220de798e017d29763fae18a691d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:8-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:acfb381334c72e0f7bb37c36b8340df55d589879a2877446ee74e50759b780d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169613330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae7b2335b1dc54032ccd4305edfa59f6d9c742e080daf2241370e25739464a04`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Nov 2021 22:08:59 GMT
ADD file:8d11c56c80a6b0631722a882ffccf6c4e58297273c4e164138c0f855a670ff79 in / 
# Wed, 24 Nov 2021 22:09:00 GMT
CMD ["/bin/bash"]
# Wed, 24 Nov 2021 22:28:21 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 24 Nov 2021 22:30:34 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Wed, 24 Nov 2021 22:30:34 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 22:30:34 GMT
ENV LANG=en_US.UTF-8
# Wed, 24 Nov 2021 22:30:35 GMT
ENV JAVA_VERSION=8u312
# Wed, 24 Nov 2021 22:30:48 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:4ade2748332d656c71c6288f12ab88613792b5c90b329ffdae521095f84faf66`  
		Last Modified: Wed, 24 Nov 2021 22:09:48 GMT  
		Size: 48.3 MB (48331000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6069e51d0239f313c0aee52bbfcdf9d451dba131643e5953161b601efac3d0`  
		Last Modified: Wed, 24 Nov 2021 22:34:59 GMT  
		Size: 15.4 MB (15388482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b458d766ad9baf442ce32527b5826441b3ccbcaa30bf1d1e4826f1578902f228`  
		Last Modified: Wed, 24 Nov 2021 22:38:03 GMT  
		Size: 105.9 MB (105893848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:344ef164090cf368920da3a4d9a21a0d59dfd454719f3bcc2d9af971fde89d45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.3 MB (170265747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a36a97dfd58802245738db39aec8ecb1a19c40d4600d856634eb9844216522e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Oct 2021 01:44:12 GMT
ADD file:f997c704e003e7bef1e40d457d005aa07a60cb4c37255cc2711119deb3e6df7d in / 
# Thu, 28 Oct 2021 01:44:13 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 02:16:09 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 28 Oct 2021 02:21:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Thu, 28 Oct 2021 02:21:13 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 02:21:14 GMT
ENV LANG=en_US.UTF-8
# Thu, 28 Oct 2021 02:21:15 GMT
ENV JAVA_VERSION=8u312
# Thu, 28 Oct 2021 02:21:38 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
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
	-	`sha256:c1db67d7024968fe76caa5aec6fc4ef19785265ad080ddc5f7ae412041ed79db`  
		Last Modified: Thu, 28 Oct 2021 02:36:07 GMT  
		Size: 104.9 MB (104906290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
