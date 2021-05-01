## `openjdk:8-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:ea0a437c84e36803bbc3a9ac7e5371d98ed0f9c44ea147f3b2cac5a96c70d05a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:8-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:a32c4207fd7e95cea88d93c27adef70e1d2551b6616ef51ceb268b0dc2a4c3d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169521156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae64b4c3374587be148eabcfc2ff785c84a205f9841419c0c545ae3960b4377b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Mar 2021 00:21:32 GMT
ADD file:837f2bca2cab135736ad43644356710dcac6516fdfc2023d239d157d1fa4ba7c in / 
# Wed, 17 Mar 2021 00:21:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Mar 2021 00:38:33 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 17 Mar 2021 00:41:39 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Wed, 17 Mar 2021 00:41:39 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Mar 2021 00:41:39 GMT
ENV LANG=en_US.UTF-8
# Wed, 21 Apr 2021 21:55:48 GMT
ENV JAVA_VERSION=8u292
# Wed, 21 Apr 2021 21:55:55 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_linux_8u292b10.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:401a42e1eb4fe87d89990847d6ef97767b5ac57457c8001203ee2ea137736907`  
		Last Modified: Wed, 17 Mar 2021 00:22:34 GMT  
		Size: 48.3 MB (48263709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f752366003eed4ac964ebb4be3453e3f19d854828f4f50ff708900bb4c42924`  
		Last Modified: Wed, 17 Mar 2021 00:45:21 GMT  
		Size: 15.4 MB (15429957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b72b904a00d0bc3de7fad6e9ababe324f7aace1d85b4bd52c80003962925811`  
		Last Modified: Wed, 21 Apr 2021 22:05:47 GMT  
		Size: 105.8 MB (105827490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:3c03b01200ccf049bd32bd0df73e43b3d27eb3c2db826a55e0d16c96f69f0b35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170227433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e62df46fee807dbf8d2f4f19bf5b2e222a5e44bd4b913391e0ff1ebb0d23021`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 01 May 2021 02:34:14 GMT
ADD file:f71ab8aa2d773f52af43dee8a58345e3c64f23cf6dc9722fc2116449655ca0ce in / 
# Sat, 01 May 2021 02:34:16 GMT
CMD ["/bin/bash"]
# Sat, 01 May 2021 02:59:26 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Sat, 01 May 2021 03:02:50 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Sat, 01 May 2021 03:02:51 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 May 2021 03:02:52 GMT
ENV LANG=en_US.UTF-8
# Sat, 01 May 2021 03:02:53 GMT
ENV JAVA_VERSION=8u292
# Sat, 01 May 2021 03:03:10 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_linux_8u292b10.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:dbfc55cb74dd07b793cdc9b4bc835fcfdb6091dad8e24cd2a6fe84ec70a2c3a6`  
		Last Modified: Sat, 01 May 2021 02:35:18 GMT  
		Size: 48.9 MB (48874038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0431cdcee2306a17be0ad5fd6791cd432218c8671e4eb75ea3a708d15ef0c6c4`  
		Last Modified: Sat, 01 May 2021 03:07:27 GMT  
		Size: 16.5 MB (16472881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f65570faef8e7fa4c63c66dc4c237b8859240799602c646eee60cd6523bd992`  
		Last Modified: Sat, 01 May 2021 03:11:44 GMT  
		Size: 104.9 MB (104880514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
