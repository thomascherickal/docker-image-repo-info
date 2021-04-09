## `openjdk:17-ea-17-oracle`

```console
$ docker pull openjdk@sha256:2bc718d7bddeb8d5767ba7ceb6442653ff4fd287da7f0413572721d97336d0af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-ea-17-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:93b2abecf523ad12e0698d1f386c9cd23ba25e3a38bada0c5f7267a52f1a3bca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241292560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f513917968be26b5c72782c637f646bbeb1c1b70eeb6a0a8642b2161d6e5f397`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 30 Mar 2021 21:01:16 GMT
ADD file:6a8b1c26fdbf2beb390286575735d9efcd8cd6c3d135c9d7d25b3fe4c641a7ee in / 
# Tue, 30 Mar 2021 21:01:16 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 21:36:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 30 Mar 2021 21:36:55 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Tue, 30 Mar 2021 21:36:55 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Mar 2021 21:36:55 GMT
ENV LANG=C.UTF-8
# Fri, 09 Apr 2021 18:55:00 GMT
ENV JAVA_VERSION=17-ea+17
# Fri, 09 Apr 2021 18:55:11 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='a53ace955971ef1ad745c2e9fef7f76b57b51d57e7076dd3a55243ab65febf87'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='ccd8ee7bb908835e697ebae8dbe38d2cf68d9f266e2d9787bdf34d26da30e45b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 09 Apr 2021 18:55:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:50c2d151af498a24eabbdd1f14042e94106189e17f7858fa9c9e6537816bfa34`  
		Last Modified: Tue, 30 Mar 2021 21:02:23 GMT  
		Size: 42.1 MB (42065616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26bc0351d047f744512b1f8920863854334f02e11637445a710596e8d9aaa7d`  
		Last Modified: Tue, 30 Mar 2021 21:43:00 GMT  
		Size: 13.3 MB (13265630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f018ef68e5276ab83b7d2768cf110a01993f06c323f19daaf2445dc5128743`  
		Last Modified: Fri, 09 Apr 2021 19:01:03 GMT  
		Size: 186.0 MB (185961314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-17-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b3244ea1c71fefd6b3759b24c08d35101fb00a319382349000e221d40b8f1ad0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.0 MB (238038237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c87af8932d98dd8692b57a61eaf3205877cb8643d84ce86d90f2ea1bdf8fca7b`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 30 Mar 2021 20:50:28 GMT
ADD file:a59a6e0ab925ce07b112d2a2ec9d3f239ea833dc65666a0d1d898d3b048c96ef in / 
# Tue, 30 Mar 2021 20:50:31 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 21:34:57 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 30 Mar 2021 21:34:58 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Tue, 30 Mar 2021 21:34:59 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Mar 2021 21:35:00 GMT
ENV LANG=C.UTF-8
# Fri, 09 Apr 2021 18:40:15 GMT
ENV JAVA_VERSION=17-ea+17
# Fri, 09 Apr 2021 18:41:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='a53ace955971ef1ad745c2e9fef7f76b57b51d57e7076dd3a55243ab65febf87'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='ccd8ee7bb908835e697ebae8dbe38d2cf68d9f266e2d9787bdf34d26da30e45b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 09 Apr 2021 18:41:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7da3223bdf8ee9e05ea4db775be9cb26ab65169aba0ba04ec2c3e0fa7331f0a2`  
		Last Modified: Tue, 30 Mar 2021 20:51:50 GMT  
		Size: 42.0 MB (41995846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e536b6ea357fbefc427ef10b23569012130790959e996d73efed97a345522cf`  
		Last Modified: Tue, 30 Mar 2021 21:41:18 GMT  
		Size: 14.0 MB (14033795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ed2acd7e43d0605a7204b49277996296ffc878c9d3ca5af3549275ce47760c`  
		Last Modified: Fri, 09 Apr 2021 18:47:19 GMT  
		Size: 182.0 MB (182008596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
