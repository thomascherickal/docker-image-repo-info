## `openjdk:19-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:92c6625d9826192743507778c6409390ef46cac6d055c6a7af7473cecb0fde02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:fd090db3951a7359304985d96d124667f45aa94441a0044c42e1018c8c93cab0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.2 MB (253226092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fddf43031f64c1372141f91f10772db494c0f7dc13c04c7980ed5ff2847555e6`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 02 Dec 2021 03:36:07 GMT
ADD file:f1e23cb77895c4f36fa773b22bdbd74dfd2a144a4da854f13fd100d73f5517d8 in / 
# Thu, 02 Dec 2021 03:36:07 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 11:28:23 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 14 Dec 2021 01:41:26 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 14 Dec 2021 01:41:26 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Dec 2021 01:41:27 GMT
ENV LANG=en_US.UTF-8
# Mon, 27 Dec 2021 18:51:52 GMT
ENV JAVA_VERSION=19-ea+3
# Mon, 27 Dec 2021 18:52:03 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/3/GPL/openjdk-19-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='30e778f7957c2a472df602c7daf108b4cc7994815c5d57bb33a90b55c70e85ca'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/3/GPL/openjdk-19-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='b984d67b32bfc13899f25f728f8c8184aac8f9e15f35d6db1f285a714eeb0234'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 27 Dec 2021 18:52:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f09c1d3b7e7b9dae0fc06393c0a6ae2becfdaf108965c4634fb5aa08ef682b39`  
		Last Modified: Thu, 02 Dec 2021 03:37:01 GMT  
		Size: 48.3 MB (48330617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a0bdeb652c6947210f8fca8bc5216da702dcb944e14fb6272fde14a87c1834`  
		Last Modified: Thu, 02 Dec 2021 11:46:03 GMT  
		Size: 15.4 MB (15388709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fe203cf35289badadca5ad2b3a0f851cd28fe866bf1094d790e9146d7f07a6`  
		Last Modified: Mon, 27 Dec 2021 19:01:19 GMT  
		Size: 189.5 MB (189506766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:2a153249db9be31878ec88276d674360c0b738a59dfd0c54c910db78830dd97c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.8 MB (253800277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea1562aba7daf51317646e0f802fae9cc233ca571269da2013d4ff96e9f0457`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 02 Dec 2021 08:51:25 GMT
ADD file:9e54130641553fdfd5c6fccb94502b8821e5f6a3a312a5b58537b439bf8b2670 in / 
# Thu, 02 Dec 2021 08:51:26 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 11:01:07 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 14 Dec 2021 01:59:08 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 14 Dec 2021 01:59:09 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Dec 2021 01:59:10 GMT
ENV LANG=en_US.UTF-8
# Mon, 27 Dec 2021 17:44:08 GMT
ENV JAVA_VERSION=19-ea+3
# Mon, 27 Dec 2021 17:44:24 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/3/GPL/openjdk-19-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='30e778f7957c2a472df602c7daf108b4cc7994815c5d57bb33a90b55c70e85ca'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/3/GPL/openjdk-19-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='b984d67b32bfc13899f25f728f8c8184aac8f9e15f35d6db1f285a714eeb0234'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 27 Dec 2021 17:44:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:badc99e3da86862c7fae71e717cef8fd1a5a34023f0932c8c979275fb8de6a32`  
		Last Modified: Thu, 02 Dec 2021 08:52:20 GMT  
		Size: 48.9 MB (48905570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56494d755d6c4fa6e0ed158c6946591b3ec2ad7e02e9c86d1434bcf5b27c263`  
		Last Modified: Thu, 02 Dec 2021 11:21:55 GMT  
		Size: 16.5 MB (16464679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe7b53e7f48b02c5d29fe6277d82ca65c21474f7f315e0ec395f443ca430c60`  
		Last Modified: Mon, 27 Dec 2021 18:00:33 GMT  
		Size: 188.4 MB (188430028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
