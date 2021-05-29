## `openjdk:11-oraclelinux8`

```console
$ docker pull openjdk@sha256:6895f77633f6eb4f51b57e39d16dfbf7095bb7f10c90876a6b35c4bbbb8aa4bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:11-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:e256bb5a8ed34ada4663b091f565eda426c2319a0e0b414ecd6aa9f6b0d7402b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258401337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb991db254b9753ae457d152315cdfa3b81cfea85a2cd7c4cc129694509ce85`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 28 May 2021 18:22:12 GMT
ADD file:9e4bcf8e1c3b7657912e93a0b82bf37752a310fa3041ec461562c85d65529ad3 in / 
# Fri, 28 May 2021 18:22:12 GMT
CMD ["/bin/bash"]
# Fri, 28 May 2021 18:39:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 28 May 2021 18:40:24 GMT
ENV JAVA_HOME=/usr/java/openjdk-11
# Fri, 28 May 2021 18:40:24 GMT
ENV PATH=/usr/java/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 May 2021 18:40:24 GMT
ENV LANG=C.UTF-8
# Fri, 28 May 2021 18:40:25 GMT
ENV JAVA_VERSION=11.0.11+9
# Fri, 28 May 2021 18:40:39 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_linux_11.0.11_9.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 28 May 2021 18:40:40 GMT
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
	-	`sha256:e876d89f85ab39a5eea956554213e41df74f92424955e3736a08534bce08c47c`  
		Last Modified: Fri, 28 May 2021 18:47:10 GMT  
		Size: 202.8 MB (202817218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:e1466c6c6a312c0cb2bf1139222e944ad42581a9f792474cd635da95d2d32faa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.7 MB (256665440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5faafbc57720cf5cfa003a6ab1b0ad4447daefc9e0616737b5f216b02b7f6a11`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 28 May 2021 18:41:46 GMT
ADD file:11d6c70bf365c2598abfb596f813afaa1a3030212b79ad6c9e239dc94fdd932a in / 
# Fri, 28 May 2021 18:41:47 GMT
CMD ["/bin/bash"]
# Fri, 28 May 2021 18:59:41 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 28 May 2021 19:02:48 GMT
ENV JAVA_HOME=/usr/java/openjdk-11
# Fri, 28 May 2021 19:02:48 GMT
ENV PATH=/usr/java/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 May 2021 19:02:48 GMT
ENV LANG=C.UTF-8
# Fri, 28 May 2021 19:02:48 GMT
ENV JAVA_VERSION=11.0.11+9
# Fri, 28 May 2021 19:03:00 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_linux_11.0.11_9.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 28 May 2021 19:03:01 GMT
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
	-	`sha256:e003caa526c5de43aa1f6fe4a302b6a3f9a5ac42c9deaed15c0b7e90132c066c`  
		Last Modified: Fri, 28 May 2021 19:16:39 GMT  
		Size: 200.4 MB (200437588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
