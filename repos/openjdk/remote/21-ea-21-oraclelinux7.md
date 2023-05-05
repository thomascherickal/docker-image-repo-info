## `openjdk:21-ea-21-oraclelinux7`

```console
$ docker pull openjdk@sha256:f9310d4bae3f9f0f26e73b5ff1870206da9943ee7de2d57f3c9791056db51cee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-21-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:1799d9d52cdddd66f9995a132ed1b043520ceed717f21b43df14ba2b38704d79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.6 MB (266596701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd4ebc8dda5cf2992526ac1126e6a44cda5919a076cc462d8a4aa8687395e69b`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 Mar 2023 22:29:01 GMT
ADD file:a14b5a8b8b6993aeee5ac6052fdf283560d65365e5bcf133ab21c4756439384a in / 
# Fri, 31 Mar 2023 22:29:01 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 23:12:41 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 31 Mar 2023 23:12:42 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 31 Mar 2023 23:12:42 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 31 Mar 2023 23:12:42 GMT
ENV LANG=en_US.UTF-8
# Thu, 04 May 2023 23:36:46 GMT
ENV JAVA_VERSION=21-ea+21
# Thu, 04 May 2023 23:36:55 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='218aa2d9ef829851d8eafe470922cefd372aa31b68cdab3aa0691c0492e6adde'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='449a26a88e27c331c9565a95892533f33792094f23f28a71b880a60588ddf0c2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 04 May 2023 23:36:56 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e83e8f2e82cc31391cd0cb4f5ba574ba5eb9708fc0f5dcc34fef53b03ef28f31`  
		Last Modified: Fri, 31 Mar 2023 22:30:40 GMT  
		Size: 50.5 MB (50496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7475b337670740c8f411f4efcbf2d4308101210ec581e69836860ffcd789ca`  
		Last Modified: Fri, 31 Mar 2023 23:14:05 GMT  
		Size: 14.2 MB (14240731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10724cb9bccb6c5606ad74ff4b1e9a800a92469420f5c890b9704240ac4e66f9`  
		Last Modified: Thu, 04 May 2023 23:39:22 GMT  
		Size: 201.9 MB (201859941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-21-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c0318ce8f7a66dac0ad17948e8fa384b9d035f9eb59b9a1044dcb07e9f61ec5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.5 MB (266524215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e5110ebcf03b51ae69a09e79b61f1ab9dfba755d2790571dda1c3af3cf8a861`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 Mar 2023 21:40:35 GMT
ADD file:4fe62bcdc8f181de8e01e791570bbb89f29712a9aef0b329febd817f4fef8887 in / 
# Fri, 31 Mar 2023 21:40:36 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 22:08:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 31 Mar 2023 22:08:06 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 31 Mar 2023 22:08:06 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 31 Mar 2023 22:08:06 GMT
ENV LANG=en_US.UTF-8
# Fri, 05 May 2023 00:02:29 GMT
ENV JAVA_VERSION=21-ea+21
# Fri, 05 May 2023 00:02:41 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='218aa2d9ef829851d8eafe470922cefd372aa31b68cdab3aa0691c0492e6adde'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='449a26a88e27c331c9565a95892533f33792094f23f28a71b880a60588ddf0c2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 05 May 2023 00:02:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a138fe98397d054834e86c902a0b929bd7cf0261ac671e779f872176569996ab`  
		Last Modified: Fri, 31 Mar 2023 21:42:01 GMT  
		Size: 51.1 MB (51054832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61213d9405aef8db0237e9542508819c698c4d8293ccbd8799a36206032fdd7c`  
		Last Modified: Fri, 31 Mar 2023 22:09:32 GMT  
		Size: 15.2 MB (15237973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8ab0c60c0fcde4d0fe5760764f395d9d0675ca7027b0d53292b8048e39a796`  
		Last Modified: Fri, 05 May 2023 00:05:03 GMT  
		Size: 200.2 MB (200231410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
