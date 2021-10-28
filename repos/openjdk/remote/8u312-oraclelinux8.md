## `openjdk:8u312-oraclelinux8`

```console
$ docker pull openjdk@sha256:b57b70ce58a14cdfe78bb2ed35d7e89415d392ccaf697046fe5a53e36da35b27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:8u312-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:17a0492759523dbd1a7cea92fd02fbde6d27fa9c8d14a6bd5954969472739e1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.4 MB (161357568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0f88085ff5f62611f6cbd12a4854c2e97af260d393237a24c105ec30ad49d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Oct 2021 01:22:47 GMT
ADD file:45a1eba89256c6e3801f14738faca9e260b17b306f0fc8769ba0b0f94f0fdf68 in / 
# Thu, 28 Oct 2021 01:22:47 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 01:44:41 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 28 Oct 2021 01:48:01 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Thu, 28 Oct 2021 01:48:01 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:48:01 GMT
ENV LANG=C.UTF-8
# Thu, 28 Oct 2021 01:48:01 GMT
ENV JAVA_VERSION=8u312
# Thu, 28 Oct 2021 01:48:11 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:f420596490555ff89c8ec7d6b74b4e46c2b3b98dc775c9d19494d8afeb475852`  
		Last Modified: Thu, 28 Oct 2021 01:24:04 GMT  
		Size: 42.0 MB (41970837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a9c63ed3ba0226d765a092dd6fcc06fe5ece8a2dd0fd11e1add9c0ddee488e`  
		Last Modified: Thu, 28 Oct 2021 01:52:24 GMT  
		Size: 13.5 MB (13491622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862d6d324cb1a810d9a0d996c35c689ccc3f61a76f6c7f8631e46f9c84a0ad7a`  
		Last Modified: Thu, 28 Oct 2021 01:57:38 GMT  
		Size: 105.9 MB (105895109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8u312-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:277d6129b971773ea1b3908802e6b2016ae8f34aec2eaaee67710513d72aae2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.1 MB (161053983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ff50808846d0f5a600dcfc45f977dc618e72dee64149ca0f3a923929fcfe637`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 14 Oct 2021 03:43:23 GMT
ADD file:f161e88dde917cf9d761056277b85a1880719b445048fc52649306cec001db66 in / 
# Thu, 14 Oct 2021 03:43:24 GMT
CMD ["/bin/bash"]
# Thu, 14 Oct 2021 05:42:19 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 14 Oct 2021 05:49:01 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Thu, 14 Oct 2021 05:49:02 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Oct 2021 05:49:03 GMT
ENV LANG=C.UTF-8
# Fri, 22 Oct 2021 02:23:43 GMT
ENV JAVA_VERSION=8u312
# Fri, 22 Oct 2021 02:23:52 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:a1eec3e47437e3334dd709f3a36be617982ec7579fa52be305301bb95c0d4be1`  
		Last Modified: Thu, 14 Oct 2021 03:44:37 GMT  
		Size: 41.9 MB (41877085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ec5552a84ea6485845e8e0a4d9b09b5e8f78d742440c18650d1ec9b1aacd89`  
		Last Modified: Thu, 14 Oct 2021 05:57:59 GMT  
		Size: 14.3 MB (14270572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97eaedc9aaad4e465fc5cdaddb05ce2cd6631a8bb88056d50dfa5d286849a4d0`  
		Last Modified: Fri, 22 Oct 2021 02:44:30 GMT  
		Size: 104.9 MB (104906326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
