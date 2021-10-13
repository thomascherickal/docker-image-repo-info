## `openjdk:11-oraclelinux7`

```console
$ docker pull openjdk@sha256:46f35d0c0f1a02f6e1d628203f3f221d689937042cc071dafafe1d3ae62b8c56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:11-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:373dbfe66a63701af88dc390a85ff401ed4937ff56e9958b957425d04e86138e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.7 MB (266689760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a00c9db28fb5dbdee7a2327183878c1dac4bd81bd31f2897f7c437b0ab1a0566`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 29 Sep 2021 16:28:42 GMT
ADD file:a9e7957ff3541c254a266620f438cb7ec181b31d50f939d0e687716cefdc7cf8 in / 
# Wed, 29 Sep 2021 16:28:43 GMT
CMD ["/bin/bash"]
# Wed, 29 Sep 2021 16:54:15 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 29 Sep 2021 16:56:52 GMT
ENV JAVA_HOME=/usr/java/openjdk-11
# Wed, 29 Sep 2021 16:56:52 GMT
ENV PATH=/usr/java/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 16:56:52 GMT
ENV LANG=en_US.UTF-8
# Wed, 29 Sep 2021 16:56:52 GMT
ENV JAVA_VERSION=11.0.12
# Wed, 29 Sep 2021 16:57:08 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 29 Sep 2021 16:57:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2294629c97e56d38612a31e50aa9a544bb9ea9a60646d016dcde035fd309dfe8`  
		Last Modified: Wed, 29 Sep 2021 16:30:26 GMT  
		Size: 48.2 MB (48241319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa27d00ff441932dc4be9fc9662577510adff660e4486fa443768e0ca6d260e`  
		Last Modified: Wed, 29 Sep 2021 17:03:16 GMT  
		Size: 15.4 MB (15433173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974f89ba561623f7855f97fd24507bda39e36d3e4a08c40981ab90d64ebf954c`  
		Last Modified: Wed, 29 Sep 2021 17:08:12 GMT  
		Size: 203.0 MB (203015268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7397cc2ff09435326dfa78aa7c39b1eabc4eda56dcc8ca3e91dc3e907c9ad599
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.9 MB (265879920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2c7623741c81d40020fc35fc8fe5d7d7e83a55ef8ca723e1520ad0925010fe2`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 29 Sep 2021 09:28:50 GMT
ADD file:affde62a0aaf80f490cc93e1f691166a15a32c6ef6bc21af35a6659d24c8b6ef in / 
# Wed, 29 Sep 2021 09:28:51 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 05:59:43 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 13 Oct 2021 06:07:57 GMT
ENV JAVA_HOME=/usr/java/openjdk-11
# Wed, 13 Oct 2021 06:07:58 GMT
ENV PATH=/usr/java/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 06:07:59 GMT
ENV LANG=en_US.UTF-8
# Wed, 13 Oct 2021 06:08:00 GMT
ENV JAVA_VERSION=11.0.12
# Wed, 13 Oct 2021 06:08:45 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 13 Oct 2021 06:08:45 GMT
CMD ["jshell"]
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
	-	`sha256:23036996dd343d28521820fcd9ac0196113177385e6bcb827bedda0de367d3a3`  
		Last Modified: Wed, 13 Oct 2021 06:37:33 GMT  
		Size: 200.6 MB (200612378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
