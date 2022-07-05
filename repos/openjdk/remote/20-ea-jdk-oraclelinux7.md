## `openjdk:20-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:05483425c5479a9430e7830904e92ce324f46534ef61a18e733435912fb4ae2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:e2a3b9b735d875a3a569433788c2e071f2ef2f9d15882082d0ffaca92a52c6b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.7 MB (259740438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5f39fdfcfc3d8d85b4d7099ead3a62942490787e07b0a88d36d56e4b291eb93`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:58 GMT
ADD file:50fb7d83a9d57e5a0a6af5e5daf27e464ae8a28c196ce6bad6c254dfc1774cdd in / 
# Tue, 05 Jul 2022 22:20:58 GMT
CMD ["/bin/bash"]
# Tue, 05 Jul 2022 22:50:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 05 Jul 2022 22:50:16 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Tue, 05 Jul 2022 22:50:16 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Jul 2022 22:50:16 GMT
ENV LANG=en_US.UTF-8
# Tue, 05 Jul 2022 22:50:16 GMT
ENV JAVA_VERSION=20-ea+4
# Tue, 05 Jul 2022 22:50:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/4/GPL/openjdk-20-ea+4_linux-x64_bin.tar.gz'; 			downloadSha256='74243a1b83dde07c3645cd0c7c3b00135fb9ca38c357e284560bf5be45a864d6'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/4/GPL/openjdk-20-ea+4_linux-aarch64_bin.tar.gz'; 			downloadSha256='ce9dd88462c6fb6c6e8be53151164b95a738e03d28788f3fd64e0339dee96de1'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 05 Jul 2022 22:50:26 GMT
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
	-	`sha256:d5ade438960d9bb3fab5b92cfc5066dd71dd6674813151abe76afc3b59902892`  
		Last Modified: Tue, 05 Jul 2022 22:59:02 GMT  
		Size: 196.7 MB (196731764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:ca6c2d46675acf707bc94a6a0e974cb7b53a7ce6a4a8416f4d0fd6e35ae996f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.2 MB (260191903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:093faeb8940ad9ce0f5e6e74b46f593d74d9e07ec6a68d8e43d5e9a8661a2794`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:37 GMT
ADD file:6d5eeb6c0921661dff8e0b6a89c3272aa52f72b5926d62ae482a85c8ef6458a3 in / 
# Tue, 05 Jul 2022 22:43:38 GMT
CMD ["/bin/bash"]
# Tue, 05 Jul 2022 23:05:04 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 05 Jul 2022 23:05:04 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Tue, 05 Jul 2022 23:05:05 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Jul 2022 23:05:06 GMT
ENV LANG=en_US.UTF-8
# Tue, 05 Jul 2022 23:05:07 GMT
ENV JAVA_VERSION=20-ea+4
# Tue, 05 Jul 2022 23:05:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/4/GPL/openjdk-20-ea+4_linux-x64_bin.tar.gz'; 			downloadSha256='74243a1b83dde07c3645cd0c7c3b00135fb9ca38c357e284560bf5be45a864d6'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/4/GPL/openjdk-20-ea+4_linux-aarch64_bin.tar.gz'; 			downloadSha256='ce9dd88462c6fb6c6e8be53151164b95a738e03d28788f3fd64e0339dee96de1'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 05 Jul 2022 23:05:26 GMT
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
	-	`sha256:fb71657283382ca761194c942ab917a3d29adaf8ef157fedda40241ffd9ba92e`  
		Last Modified: Tue, 05 Jul 2022 23:22:09 GMT  
		Size: 195.6 MB (195584631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
