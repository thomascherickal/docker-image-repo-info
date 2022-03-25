## `openjdk:8u322-oraclelinux7`

```console
$ docker pull openjdk@sha256:f6bd3090549a53171b14c416e8a9e6d468d8f0862df0aecbbf620326275a89f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:8u322-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:b47c62fa7ecb95f07c137ee4d96b35ef3a93a74980fad3e7deb4b47783540617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.9 MB (168944722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86ae4197e3e1d22fccfff6c5710e702217408c6be3a4e88a740248b0f8bd3371`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 24 Mar 2022 22:26:41 GMT
ADD file:c54c465abf0c60dc924ca0809a1a862121214379efe90dacb9c9947c81054213 in / 
# Thu, 24 Mar 2022 22:26:42 GMT
CMD ["/bin/bash"]
# Fri, 25 Mar 2022 01:17:16 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 25 Mar 2022 01:20:23 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Fri, 25 Mar 2022 01:20:23 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 25 Mar 2022 01:20:23 GMT
ENV LANG=en_US.UTF-8
# Fri, 25 Mar 2022 01:20:24 GMT
ENV JAVA_VERSION=8u322
# Fri, 25 Mar 2022 01:20:30 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:fda5369ef22868b2225eb458f776aabaf140371e2f8d709c4de99b69a02ae748`  
		Last Modified: Thu, 24 Mar 2022 22:28:00 GMT  
		Size: 48.7 MB (48749451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175ebd0783e9e11a5749d6a07553e79af5cce82b84020eca354389f2e772070e`  
		Last Modified: Fri, 25 Mar 2022 01:25:40 GMT  
		Size: 14.2 MB (14229382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b248addebcae5767d0f1e299351a9ddd8cd33e4e174741f2385c203c3c480fd6`  
		Last Modified: Fri, 25 Mar 2022 01:32:04 GMT  
		Size: 106.0 MB (105965889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8u322-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:4454b5991ac96fe0273e71c7886161a1247d46746c6d338f8226e30cfcfa56b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169592437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e717c7fe71eccf8d81a91912fc2f0f04596a885c3e0531fc4c2ae5909c685ea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 24 Mar 2022 22:21:33 GMT
ADD file:458f691e62c6797d5a132b3af3e3d34358f4563c2f767879ff5a5edaac9c76ee in / 
# Thu, 24 Mar 2022 22:21:34 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 22:46:20 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 24 Mar 2022 22:52:22 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Thu, 24 Mar 2022 22:52:23 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 22:52:24 GMT
ENV LANG=en_US.UTF-8
# Thu, 24 Mar 2022 22:52:25 GMT
ENV JAVA_VERSION=8u322
# Thu, 24 Mar 2022 22:52:48 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:3a4f104bbb26007de614fa29a9ed91e9210287087323d3de394a39f0d9f1139c`  
		Last Modified: Thu, 24 Mar 2022 22:23:06 GMT  
		Size: 49.3 MB (49340038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a5491893ff1eefd4a92b9f85621f8ee58a84cb7d0fa6edf8ca55ed7dad5724`  
		Last Modified: Thu, 24 Mar 2022 23:02:13 GMT  
		Size: 15.3 MB (15270343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03003bd16cae5d28885f836a3f1fc0c85f190c165bd2d97829d3dbbde127c529`  
		Last Modified: Thu, 24 Mar 2022 23:10:13 GMT  
		Size: 105.0 MB (104982056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
