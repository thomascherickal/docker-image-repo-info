## `openjdk:8-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:2606c6ad18bcb8cd969934cfe48eb08ff9842dd2346f72766397c4f7e531f1a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:8-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:e649c2299d811e3f6d580f38a8d84f33d5f736a70817aaa15ec06760559275f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169516609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:361aff43363f1c718048994a911964eda679ef39aee4822e9cbc5e8881a2b3c5`
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
# Wed, 13 Oct 2021 18:52:22 GMT
ENV JAVA_VERSION=8u302
# Wed, 13 Oct 2021 18:52:36 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
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
	-	`sha256:5f03d238eeee6f718515d8b528461a2ea655f92103f556bdd4920be77254e306`  
		Last Modified: Wed, 13 Oct 2021 19:03:53 GMT  
		Size: 105.9 MB (105882887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:3c0c93918cbc5a491107181bf7cd0b7a91bf71a03dcb4c3caae8c019126d37a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170165522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88b7b8dd078dcbef4da625004fd800c02a022fc89be860782e79440ef4a12acf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 29 Sep 2021 09:28:50 GMT
ADD file:affde62a0aaf80f490cc93e1f691166a15a32c6ef6bc21af35a6659d24c8b6ef in / 
# Wed, 29 Sep 2021 09:28:51 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 05:59:43 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 13 Oct 2021 06:13:09 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Wed, 13 Oct 2021 06:13:10 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 06:13:11 GMT
ENV LANG=en_US.UTF-8
# Wed, 13 Oct 2021 06:13:12 GMT
ENV JAVA_VERSION=8u302
# Wed, 13 Oct 2021 06:13:32 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:2f5eee715870559160403451bcd7b891478e0df052b7f9456144f3e89e5b994f`  
		Last Modified: Wed, 29 Sep 2021 09:30:28 GMT  
		Size: 48.8 MB (48828923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d586374e21f8d72195ddee3ded7c701588c9aaf00feb9feeaf6a586f435121df`  
		Last Modified: Wed, 13 Oct 2021 06:24:14 GMT  
		Size: 16.4 MB (16438619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb0a0b93bde7f82dd93e2be313d60ac92c4b72591310b4d6787a0ce5e81bc83`  
		Last Modified: Wed, 13 Oct 2021 06:43:20 GMT  
		Size: 104.9 MB (104897980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
