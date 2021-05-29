## `openjdk:17-oraclelinux8`

```console
$ docker pull openjdk@sha256:d50231b3997fc205419425c565e7a6e992ec35ecbd2d6068052a72bb3996584f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:136f5625d48e7b826984c7a105c1859c97472db139bb65767c65aecd2645264d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241816735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d3d45e079769c5f6b6484e9bc4c52848f99dbdddc418ad2a6678fd05049522c`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 28 May 2021 18:22:12 GMT
ADD file:9e4bcf8e1c3b7657912e93a0b82bf37752a310fa3041ec461562c85d65529ad3 in / 
# Fri, 28 May 2021 18:22:12 GMT
CMD ["/bin/bash"]
# Fri, 28 May 2021 18:39:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 28 May 2021 18:39:11 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 28 May 2021 18:39:11 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 May 2021 18:39:12 GMT
ENV LANG=C.UTF-8
# Fri, 28 May 2021 18:39:12 GMT
ENV JAVA_VERSION=17-ea+24
# Fri, 28 May 2021 18:39:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/24/GPL/openjdk-17-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='30b8cc8945c42ab310bca47ecfe2acdf2a0285d26dfeb6bfba46ebc5947aef6e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/24/GPL/openjdk-17-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='61d192356099180ee3beec3a22cb9e97cb810c7f55f2c870a73841c3ac61abcb'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 28 May 2021 18:39:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:daa797b1cf01195cd47497fc9ddbf3fc4404f3fc012110f206b7fa3dd531e43d`  
		Last Modified: Fri, 28 May 2021 18:23:25 GMT  
		Size: 42.2 MB (42183040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7f736a217a7dd2e90a8ba647050e6374f7c3f746ad3256682302739a73ee7`  
		Last Modified: Fri, 28 May 2021 18:44:27 GMT  
		Size: 13.4 MB (13401079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f5d5c2a12a1ad5ac657bacf748f311f11f1e1c905d2fd30b0b3c83cea7be20`  
		Last Modified: Fri, 28 May 2021 18:44:45 GMT  
		Size: 186.2 MB (186232616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:ac493e87d3033e8da76316e7ccff86628eaad00ce0b9248be94d1fb2c41edbee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.5 MB (238518694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ffbdf114980656793db81c532e06feb06f2e3e7aa25ede71e10711243b9835`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 28 May 2021 18:41:46 GMT
ADD file:11d6c70bf365c2598abfb596f813afaa1a3030212b79ad6c9e239dc94fdd932a in / 
# Fri, 28 May 2021 18:41:47 GMT
CMD ["/bin/bash"]
# Fri, 28 May 2021 18:59:41 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 28 May 2021 18:59:41 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 28 May 2021 18:59:41 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 May 2021 18:59:42 GMT
ENV LANG=C.UTF-8
# Fri, 28 May 2021 18:59:42 GMT
ENV JAVA_VERSION=17-ea+24
# Fri, 28 May 2021 19:00:04 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/24/GPL/openjdk-17-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='30b8cc8945c42ab310bca47ecfe2acdf2a0285d26dfeb6bfba46ebc5947aef6e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/24/GPL/openjdk-17-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='61d192356099180ee3beec3a22cb9e97cb810c7f55f2c870a73841c3ac61abcb'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 28 May 2021 19:00:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6bb7bddcd571a468c93282c3fa3b0e38fdcf15ee58fec20d63d32da56f3074af`  
		Last Modified: Fri, 28 May 2021 18:43:06 GMT  
		Size: 42.1 MB (42054735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1363fd6ea5b7069bbb5efb69721e5fbb5c89d4cf037ed7b6b6ed1476fa5ad8`  
		Last Modified: Fri, 28 May 2021 19:11:54 GMT  
		Size: 14.2 MB (14173117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ada731f025b032e1f4109f4831d086024044046d34086e435887ba2f70c98`  
		Last Modified: Fri, 28 May 2021 19:12:10 GMT  
		Size: 182.3 MB (182290842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
