## `openjdk:15-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:d1ddd93b20030ed610f8c017f6fbeb5d35361ae21ae11c659be01a1ba0f26708
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:15-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:209f0b4cb77f4a5e9932530af62e3cd097649f5a8d5781395c618aca36a1f3ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.5 MB (259491487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d48824efa7d84e65ec6943cfb013f7b43f753e02f074ea5be1925fdf62a914b3`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 15 Jan 2021 00:31:31 GMT
ADD file:dee09ad1ed4e7359b14fabc84890b1fb687ad4efe75f7c4800c0a907fd4f70a3 in / 
# Fri, 15 Jan 2021 00:31:32 GMT
CMD ["/bin/bash"]
# Fri, 15 Jan 2021 00:58:14 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 15 Jan 2021 00:58:14 GMT
ENV LANG=en_US.UTF-8
# Fri, 15 Jan 2021 01:01:46 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 15 Jan 2021 01:01:46 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:45:43 GMT
ENV JAVA_VERSION=15.0.2
# Wed, 20 Jan 2021 00:46:02 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.2/0d1cfde4252546c6931946de8db48ee2/7/GPL/openjdk-15.0.2_linux-aarch64_bin.tar.gz; 			downloadSha256=3958f01858f9290c48c23e7804a0af3624e8eca6749b085c425df4c4f2f7dcbc; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.2/0d1cfde4252546c6931946de8db48ee2/7/GPL/openjdk-15.0.2_linux-x64_bin.tar.gz; 			downloadSha256=91ac6fc353b6bf39d995572b700e37a20e119a87034eeb939a6f24356fbcd207; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 20 Jan 2021 00:46:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:980316e412373040bc280150078ae453b259ece36b750a0a9b6f4c99751ce4f9`  
		Last Modified: Wed, 06 Jan 2021 20:24:02 GMT  
		Size: 48.3 MB (48260808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7699f318b6b854fb950c083e0fed757fff0549df020432861c6b50802ec82b2`  
		Last Modified: Fri, 15 Jan 2021 01:09:18 GMT  
		Size: 15.4 MB (15431689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf25c2399a2f3f20fa8f1ff2bc6f53049f59cd129ade2337beca62f3a5b0bb34`  
		Last Modified: Wed, 20 Jan 2021 00:53:29 GMT  
		Size: 195.8 MB (195798990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:08ff77d4c365f4e7b4c3bdce0a852bbba9d19208501764e97c676414c24d1c57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240211281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5dc74a97ee41ea551e4abfaebb65c23e0b8887edac11dc7c481947a7cf9ff0e`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 15 Jan 2021 00:06:30 GMT
ADD file:d4d5ffcc8d57e27f8de10063c4e347d2f4da299f62166d6f6387a7714f5e0f06 in / 
# Fri, 15 Jan 2021 00:06:33 GMT
CMD ["/bin/bash"]
# Fri, 15 Jan 2021 00:45:52 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 15 Jan 2021 00:45:53 GMT
ENV LANG=en_US.UTF-8
# Fri, 15 Jan 2021 00:49:31 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 15 Jan 2021 00:49:32 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:43:23 GMT
ENV JAVA_VERSION=15.0.2
# Wed, 20 Jan 2021 00:43:45 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.2/0d1cfde4252546c6931946de8db48ee2/7/GPL/openjdk-15.0.2_linux-aarch64_bin.tar.gz; 			downloadSha256=3958f01858f9290c48c23e7804a0af3624e8eca6749b085c425df4c4f2f7dcbc; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.2/0d1cfde4252546c6931946de8db48ee2/7/GPL/openjdk-15.0.2_linux-x64_bin.tar.gz; 			downloadSha256=91ac6fc353b6bf39d995572b700e37a20e119a87034eeb939a6f24356fbcd207; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 20 Jan 2021 00:43:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e2e87614faabf530f11811ae8eb1be9e586d5d923036268129a39eae319cb772`  
		Last Modified: Wed, 06 Jan 2021 20:47:54 GMT  
		Size: 48.9 MB (48858154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458e99ea3b1687330632146091a5677b179fe906820e2d98ad7b5becbcb526c1`  
		Last Modified: Fri, 15 Jan 2021 00:56:17 GMT  
		Size: 16.5 MB (16470870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646c61d16ac19363dff310341044840489cdb2abc4d046455c3686d52ad40c20`  
		Last Modified: Wed, 20 Jan 2021 00:50:24 GMT  
		Size: 174.9 MB (174882257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
