## `openjdk:11-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:4e9301cbfc9f790ea6fcd2380bec41a43922d300a259511bdf1a58d549c0f127
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:11-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:a7754958f07ecda0a7510c5c6cdc613e9ee5152b269a27413e2f3e70539c7904
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.6 MB (266645184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ad710d90b21e368b4ab694c05a0055c82f2cd57411ad2c2778b93eca4da620d`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 13 Oct 2021 18:30:19 GMT
ADD file:a6def617e1c0cf7def2d3ce3c79073621ed8efb37deed65fb49e7fc0a6d8ea37 in / 
# Wed, 13 Oct 2021 18:30:20 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 18:48:31 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 13 Oct 2021 18:51:08 GMT
ENV JAVA_HOME=/usr/java/openjdk-11
# Wed, 13 Oct 2021 18:51:08 GMT
ENV PATH=/usr/java/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 18:51:08 GMT
ENV LANG=en_US.UTF-8
# Thu, 21 Oct 2021 23:43:29 GMT
ENV JAVA_VERSION=11.0.13
# Thu, 21 Oct 2021 23:43:44 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 21 Oct 2021 23:43:45 GMT
CMD ["jshell"]
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
	-	`sha256:c661cb666b476ec61402cfb21a17faac1492b3da1d0210c41ee1b19bc1c96ffb`  
		Last Modified: Thu, 21 Oct 2021 23:58:00 GMT  
		Size: 203.0 MB (203011462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:d29dc1b4eb5623c389715995dbb2079749147fe25a5eefd3775d7297db5a7eee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.9 MB (265878827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab8986061f64e7555eb8cf4ed3cef39c83ac2efa688059d49ac1154ee47dd7cb`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 14 Oct 2021 03:43:46 GMT
ADD file:fca1474953cf608c9b2613787e7e7b859d458af91405a97dbd4ee57c63565185 in / 
# Thu, 14 Oct 2021 03:43:47 GMT
CMD ["/bin/bash"]
# Thu, 14 Oct 2021 05:43:29 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 14 Oct 2021 05:47:36 GMT
ENV JAVA_HOME=/usr/java/openjdk-11
# Thu, 14 Oct 2021 05:47:37 GMT
ENV PATH=/usr/java/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Oct 2021 05:47:38 GMT
ENV LANG=en_US.UTF-8
# Thu, 14 Oct 2021 05:47:39 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 14 Oct 2021 05:48:05 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 14 Oct 2021 05:48:06 GMT
CMD ["jshell"]
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
	-	`sha256:0bbd86bd0943ad1b84aa019df145df26feddc46eb13b71377c82e22c3d639989`  
		Last Modified: Thu, 14 Oct 2021 06:04:34 GMT  
		Size: 200.6 MB (200610973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
