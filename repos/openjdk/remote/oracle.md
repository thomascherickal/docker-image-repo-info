## `openjdk:oracle`

```console
$ docker pull openjdk@sha256:a51c72f59f74223970a911361e1427d7b69245195f74f9a73926707c0926b0a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:3defb1ab91bda238bd37f34b134e11f742c880bcaef8b4ac27b3262b3ba4bfe6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.1 MB (243144112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a85d8f6e1bdd1e28e019ee6bad7d625bdf7531fc8356bb352faf630230999beb`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Feb 2022 05:30:31 GMT
ADD file:17957b69b27e30b1d860c0919546da181b5e126b4aca4e1935ab44fd1832578e in / 
# Fri, 04 Feb 2022 05:30:31 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 06:31:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 04 Feb 2022 06:32:56 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 04 Feb 2022 06:32:56 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Feb 2022 06:32:57 GMT
ENV LANG=C.UTF-8
# Fri, 04 Feb 2022 06:32:57 GMT
ENV JAVA_VERSION=17.0.2
# Fri, 04 Feb 2022 06:33:07 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 04 Feb 2022 06:33:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f431a76c5f59c48efd4a4076677acaae2b540a7562de00075162ef8a340fd69b`  
		Last Modified: Fri, 04 Feb 2022 05:31:30 GMT  
		Size: 42.1 MB (42102405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0509e57e85d3b85eac03c20f8f88d1cb2481d6122bdae0020851f7022e3b31`  
		Last Modified: Fri, 04 Feb 2022 08:22:45 GMT  
		Size: 13.5 MB (13513973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99183953ac5d5bafa925c1b03d239d433576f5dc1cae53fee20bc6c37d09568e`  
		Last Modified: Fri, 04 Feb 2022 08:24:05 GMT  
		Size: 187.5 MB (187527734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:a3dac62b74790839fbc43043064e9ea86b63918fd47f490e82bc6c9d91b8f10a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.7 MB (242666222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2772c703eb651f7a241415bd19e66a0ff71e805fb281f22a4653cd40d394cea0`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Feb 2022 04:13:53 GMT
ADD file:22ac13d97f9f75668fec05f2cf9d182e5edcf2822b08ef38929b0bb8d61f5edb in / 
# Fri, 04 Feb 2022 04:13:54 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 05:34:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 04 Feb 2022 05:38:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 04 Feb 2022 05:38:14 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Feb 2022 05:38:15 GMT
ENV LANG=C.UTF-8
# Fri, 04 Feb 2022 05:38:16 GMT
ENV JAVA_VERSION=17.0.2
# Fri, 04 Feb 2022 05:38:27 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 04 Feb 2022 05:38:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:200ed4b56d545919e183ba8dfa2493452065262be1759dd78c3de721a71882cb`  
		Last Modified: Fri, 04 Feb 2022 04:14:59 GMT  
		Size: 42.0 MB (42011648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4545cbf19e4d384cf8f28f10cdb2cb3e0cfb6a09f47542c1c092358c7fd1b5`  
		Last Modified: Fri, 04 Feb 2022 05:50:37 GMT  
		Size: 14.3 MB (14290526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c52ee4a32a999688ddd79222e497c2226d984006f6ec5b3bdc773ef75e033e7`  
		Last Modified: Fri, 04 Feb 2022 05:52:14 GMT  
		Size: 186.4 MB (186364048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
