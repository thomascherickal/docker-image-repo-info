## `openjdk:19-ea-14-oracle`

```console
$ docker pull openjdk@sha256:de32530f5be617bf6e3c99b4e57a575165a7107d9124158434a8a59f13190cbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-14-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:f66e9723eab0072d5903e277d78d15834c063ad95e2a40d289c093ad85e2aacd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.7 MB (248729071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26bc5c350476f5c743035c3e2f9bafa2b838bdc2734c12c5124216bc7fe5d448`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Mar 2022 01:39:10 GMT
ADD file:c0f0a367bc612431ac9286b506fef5505e0b5f3969515486d8052ec381524261 in / 
# Thu, 24 Mar 2022 01:39:10 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 01:59:03 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 24 Mar 2022 01:59:04 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 24 Mar 2022 01:59:04 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 01:59:04 GMT
ENV LANG=C.UTF-8
# Thu, 24 Mar 2022 01:59:04 GMT
ENV JAVA_VERSION=19-ea+14
# Thu, 24 Mar 2022 01:59:13 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/14/GPL/openjdk-19-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='7c64317f728ce251b1fa6fcc612bbc5e4fac4d2862cf0f9b9edd98800072b6bc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/14/GPL/openjdk-19-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='166aaa023baf2fff6484465efd16040557b4bbd57362409d730acec5d01fe749'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 24 Mar 2022 01:59:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a9d3d14d30b79ab021a558da3520be505bd2c5ab0f4c85aa07a3ed43524cea2f`  
		Last Modified: Thu, 24 Mar 2022 01:40:02 GMT  
		Size: 42.1 MB (42111482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8d91aae4872bdf5c523549a1c38e887a3d031b5f174e2e3686d0eca9415dca`  
		Last Modified: Thu, 24 Mar 2022 02:06:25 GMT  
		Size: 13.5 MB (13531708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9567c074f36b342dd1b5cd0d032a4a031e155339503d80c6f31802326e52f15`  
		Last Modified: Thu, 24 Mar 2022 02:06:38 GMT  
		Size: 193.1 MB (193085881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-14-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f555ebdfcee89b6271f21b6034e62403da7dbced1d60432cb563db26e9ecf1bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.4 MB (248429368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:292f0e5a14f0519d581ed6d95bca2746a5794edc700993d9b0da7d9e18542e86`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 18 Mar 2022 00:35:35 GMT
ADD file:b16af05882bd38ac02b1f1cba2cc7e80bfbe467ce57f3cf35f1f5a551cee90fa in / 
# Fri, 18 Mar 2022 00:35:36 GMT
CMD ["/bin/bash"]
# Sat, 19 Mar 2022 07:22:07 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 19 Mar 2022 07:22:07 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Sat, 19 Mar 2022 07:22:08 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 07:22:09 GMT
ENV LANG=C.UTF-8
# Tue, 22 Mar 2022 10:02:34 GMT
ENV JAVA_VERSION=19-ea+14
# Tue, 22 Mar 2022 10:02:52 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/14/GPL/openjdk-19-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='7c64317f728ce251b1fa6fcc612bbc5e4fac4d2862cf0f9b9edd98800072b6bc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/14/GPL/openjdk-19-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='166aaa023baf2fff6484465efd16040557b4bbd57362409d730acec5d01fe749'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 22 Mar 2022 10:02:52 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2f8e506fd7c6683f24250871efec36e3fe21cc71090a2f5c59dccdcdfeed2311`  
		Last Modified: Fri, 18 Mar 2022 00:36:38 GMT  
		Size: 42.0 MB (42017883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5fff79dab44aae745004a90eddcd68a9db24e820f0c68e482a9508464ea719`  
		Last Modified: Sat, 19 Mar 2022 07:43:39 GMT  
		Size: 14.3 MB (14291778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a47e7293c29a2389191c592de9dc220439260caa5a0d1f5c7af040e6a8e5f8`  
		Last Modified: Tue, 22 Mar 2022 10:16:13 GMT  
		Size: 192.1 MB (192119707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
