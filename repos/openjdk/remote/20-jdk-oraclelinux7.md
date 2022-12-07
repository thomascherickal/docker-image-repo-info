## `openjdk:20-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:51ad1fe7fa9e38351861c8f13ac5229b9e53401fd6f7cd7da67f6d96966d5a62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:a4a310f10bb51729e0ad7d5733324cfdcaf5d8c7f7207c17b6fea902b2bd18dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.0 MB (261986179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c21001d0145efe47fa6a921545ebc740820205cd22fca48a8c875e34d6c0d64b`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:27:36 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 07 Dec 2022 02:27:36 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 07 Dec 2022 02:27:36 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Dec 2022 02:27:36 GMT
ENV LANG=en_US.UTF-8
# Wed, 07 Dec 2022 02:27:36 GMT
ENV JAVA_VERSION=20-ea+26
# Wed, 07 Dec 2022 02:27:47 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='70075a76ed683898d8d71852394c88ab73d8665b15accfafa85dac3be5fbf87e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='041c2b0e7b68e58376d8b03db365434ceecd65671de20af28e6c32f47ccde94a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 07 Dec 2022 02:27:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13169d9a90276a4f8190fd6edcdf29f7dd28e38d5919cd950939ffe59628af48`  
		Last Modified: Wed, 07 Dec 2022 02:31:28 GMT  
		Size: 14.2 MB (14217950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bf34a7bdecacfa3c975a1c4b35f77f3d0cd9f9ee258fc24c2ca8fe3a486838`  
		Last Modified: Wed, 07 Dec 2022 02:31:41 GMT  
		Size: 197.9 MB (197949747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:378116c8d2fce918aa11cb33a0056a75865e6c23e323ff2b71bbddd6c021cce0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.2 MB (262154740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c838385ce4afdf99167bcb0605957fa2500ec8dce650f79e3ed9db4ae0064fb0`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 07 Dec 2022 02:11:05 GMT
ADD file:811a8ff51774a6c04c874e49a9bf2f3ef1a447402946740d2128a81809dc1a22 in / 
# Wed, 07 Dec 2022 02:11:06 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:53:45 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 07 Dec 2022 02:53:45 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 07 Dec 2022 02:53:45 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Dec 2022 02:53:45 GMT
ENV LANG=en_US.UTF-8
# Wed, 07 Dec 2022 02:53:45 GMT
ENV JAVA_VERSION=20-ea+26
# Wed, 07 Dec 2022 02:53:57 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='70075a76ed683898d8d71852394c88ab73d8665b15accfafa85dac3be5fbf87e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='041c2b0e7b68e58376d8b03db365434ceecd65671de20af28e6c32f47ccde94a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 07 Dec 2022 02:53:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:81ac616e14aefb691216238b73174a9efd12a5e52bc4e297c5c1cf38561e5aca`  
		Last Modified: Wed, 07 Dec 2022 02:12:40 GMT  
		Size: 50.4 MB (50386463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804baa16591d133fbd09bac6a9223716dbf71fec46b68197f09b7ad836238810`  
		Last Modified: Wed, 07 Dec 2022 02:57:50 GMT  
		Size: 15.3 MB (15268238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c54ddb2a5ed7c8b9a64fdf4e2a688266b4d778d5d16a685380e4f748e2f3f8b`  
		Last Modified: Wed, 07 Dec 2022 02:58:00 GMT  
		Size: 196.5 MB (196500039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
