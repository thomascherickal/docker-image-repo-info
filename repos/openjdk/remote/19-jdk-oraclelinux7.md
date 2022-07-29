## `openjdk:19-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:bb2931fa305b2dbb426c3280f826772e7b8b6d42a2104ec3321812a585c0fa42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:dc97a3166bd506e7fac548437141deeced60954da0c8ed0a2cc07fac37a31711
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.2 MB (259179365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00a576b8aff72bb0116af1a3f8c425de165aff8b8ce5559c3992d70e1f184278`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:58 GMT
ADD file:50fb7d83a9d57e5a0a6af5e5daf27e464ae8a28c196ce6bad6c254dfc1774cdd in / 
# Tue, 05 Jul 2022 22:20:58 GMT
CMD ["/bin/bash"]
# Tue, 05 Jul 2022 22:50:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 05 Jul 2022 22:50:56 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 05 Jul 2022 22:50:56 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Jul 2022 22:50:56 GMT
ENV LANG=en_US.UTF-8
# Fri, 29 Jul 2022 02:04:57 GMT
ENV JAVA_VERSION=19-ea+33
# Fri, 29 Jul 2022 02:05:07 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='31aa1cf0a266dfc90d9e85d688379a2b2b9b1888bb7df326a4434dc92fdc105f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='8e758bdc4cd496f29c85a53ce1eb155b7ee8f945c11517cc4a766492349c52e2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 29 Jul 2022 02:05:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:66fb3478003364657ac7751c40e41a135e02975f9459f652b1df23e3896b5fac`  
		Last Modified: Tue, 05 Jul 2022 22:22:18 GMT  
		Size: 48.8 MB (48762895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8f0f1eb3582fe120c104ded4086894e324ef46a631953f821f879e3e7a6a26`  
		Last Modified: Tue, 05 Jul 2022 22:58:49 GMT  
		Size: 14.2 MB (14245779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8435b86446bad5a093677047afd1422e19bed511dc50ea42b0ea8488b55b9aab`  
		Last Modified: Fri, 29 Jul 2022 02:16:34 GMT  
		Size: 196.2 MB (196170691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:16612062b4e152e8dc7badd20be3a830433a5967b8ac29a43edc8e1b9a413679
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259623892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9d0d5c0114fd48f199ba4367fab3db0d72b745613f37c290a3d7e6754b5263`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:37 GMT
ADD file:6d5eeb6c0921661dff8e0b6a89c3272aa52f72b5926d62ae482a85c8ef6458a3 in / 
# Tue, 05 Jul 2022 22:43:38 GMT
CMD ["/bin/bash"]
# Tue, 05 Jul 2022 23:05:04 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 05 Jul 2022 23:06:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 05 Jul 2022 23:06:34 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Jul 2022 23:06:35 GMT
ENV LANG=en_US.UTF-8
# Fri, 29 Jul 2022 02:40:00 GMT
ENV JAVA_VERSION=19-ea+33
# Fri, 29 Jul 2022 02:40:18 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='31aa1cf0a266dfc90d9e85d688379a2b2b9b1888bb7df326a4434dc92fdc105f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='8e758bdc4cd496f29c85a53ce1eb155b7ee8f945c11517cc4a766492349c52e2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 29 Jul 2022 02:40:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:456ca0cbf3e695c518e5d5c4cb5ff9f99bb999a28b5ec7da3b4ca48d3cf80e6b`  
		Last Modified: Tue, 05 Jul 2022 22:45:10 GMT  
		Size: 49.3 MB (49342729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7981fd8b8b8e53f7977497096fa392e1d14f1e3dd10684ac47d3fa4688b887e7`  
		Last Modified: Tue, 05 Jul 2022 23:21:54 GMT  
		Size: 15.3 MB (15264543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6549b576f7af5e5865745898c6d3a8dd2a730e30ff65cb68dd25aee178bde353`  
		Last Modified: Fri, 29 Jul 2022 02:58:23 GMT  
		Size: 195.0 MB (195016620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
