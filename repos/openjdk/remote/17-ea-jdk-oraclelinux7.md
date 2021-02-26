## `openjdk:17-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:057eb178ea03d74fdfec9ec8255815702ea6ed7484de6cbc1d49f46f303957c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:8b1910cd43b4c87418c6e9943f36c465ba5609a8b5552af8406df66496116ebd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.4 MB (249398422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6dcdb9792713b92cf0b012c03e653ca49570fa99e0e9c1fa1fb7a5a7595c286`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 12 Feb 2021 00:53:29 GMT
ADD file:361f165903526126476b03dd2afac1fff0b334906bb56d024e5aee87b948b0cf in / 
# Fri, 12 Feb 2021 00:53:29 GMT
CMD ["/bin/bash"]
# Fri, 12 Feb 2021 01:11:19 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 12 Feb 2021 01:11:19 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 12 Feb 2021 01:11:19 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Feb 2021 01:11:19 GMT
ENV LANG=en_US.UTF-8
# Fri, 26 Feb 2021 21:22:09 GMT
ENV JAVA_VERSION=17-ea+11
# Fri, 26 Feb 2021 21:22:23 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/11/GPL/openjdk-17-ea+11_linux-x64_bin.tar.gz'; 			downloadSha256='03f129a2a92537e3eea68a0f816baae2e97a228deb50176631d040f6895b3d78'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/11/GPL/openjdk-17-ea+11_linux-aarch64_bin.tar.gz'; 			downloadSha256='8680345eaa4cd3e14584f480f75491fd20966a6fd6c9d4a418e0ec55d9d2ed12'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Feb 2021 21:22:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a61503a3b32ea964eb926d54dcfe6cd7e21f4e0cca1b1373df21cf904388c445`  
		Last Modified: Fri, 12 Feb 2021 00:54:42 GMT  
		Size: 48.3 MB (48263629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2d02ff646cdda3eb210d43b22353e431d4fa3a204470452ad0a0508cdbf87d`  
		Last Modified: Fri, 12 Feb 2021 01:18:03 GMT  
		Size: 15.4 MB (15437000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2b41296029d05de30fbc2f2a5cc1ad29be2093757d821c5d3dbef536c61ac3`  
		Last Modified: Fri, 26 Feb 2021 21:27:59 GMT  
		Size: 185.7 MB (185697793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:ffd52e529bfc9aa89bde68f16c0e2221a0de381606a9529b4998c4bf874125ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.0 MB (247030080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97c8327e64c25f63bcf6127033b01b9c8a62b4d9aaea72b58d6b7ca04b008d1`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 12 Feb 2021 01:00:40 GMT
ADD file:25b64ec41b7ca742c671c416e08a7bee3224e4052650624ef31b5583b1c412df in / 
# Fri, 12 Feb 2021 01:00:41 GMT
CMD ["/bin/bash"]
# Fri, 12 Feb 2021 01:19:33 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 12 Feb 2021 01:19:34 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 12 Feb 2021 01:19:35 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Feb 2021 01:19:35 GMT
ENV LANG=en_US.UTF-8
# Fri, 26 Feb 2021 21:54:53 GMT
ENV JAVA_VERSION=17-ea+11
# Fri, 26 Feb 2021 21:55:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/11/GPL/openjdk-17-ea+11_linux-x64_bin.tar.gz'; 			downloadSha256='03f129a2a92537e3eea68a0f816baae2e97a228deb50176631d040f6895b3d78'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/11/GPL/openjdk-17-ea+11_linux-aarch64_bin.tar.gz'; 			downloadSha256='8680345eaa4cd3e14584f480f75491fd20966a6fd6c9d4a418e0ec55d9d2ed12'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Feb 2021 21:55:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:da6ef06bd6983a3815530ecb4b6d3bcef6c011f03daa80be12f60c382e0c23e9`  
		Last Modified: Fri, 12 Feb 2021 01:01:42 GMT  
		Size: 48.9 MB (48854102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2cbabffc67d7d6521300614c7fd34cc6a54a4697d98c388898fc060b0f77d3`  
		Last Modified: Fri, 12 Feb 2021 01:26:00 GMT  
		Size: 16.5 MB (16465019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a2c7f4a9c03f3e991d148a4babe7a562473374c592794c69f0997979bb161e`  
		Last Modified: Fri, 26 Feb 2021 22:01:02 GMT  
		Size: 181.7 MB (181710959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
