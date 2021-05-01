## `openjdk:17-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:83594420d58b6c6a789f0ad6e32ba8a86e7fb9b9fbafe99a631b866154e77a77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:c1fa21b8151341f1ce63cd7869c07934a74ef41bd6d4dd85186ff709c4320e1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.7 MB (249697474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e73ca130736244390e92313e2a0f597acde4ded27f1cadb163f8b0f8665cd49e`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 17 Mar 2021 00:21:32 GMT
ADD file:837f2bca2cab135736ad43644356710dcac6516fdfc2023d239d157d1fa4ba7c in / 
# Wed, 17 Mar 2021 00:21:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Mar 2021 00:38:33 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 17 Mar 2021 00:38:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 17 Mar 2021 00:38:34 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Mar 2021 00:38:34 GMT
ENV LANG=en_US.UTF-8
# Sat, 01 May 2021 03:39:24 GMT
ENV JAVA_VERSION=17-ea+20
# Sat, 01 May 2021 03:39:35 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='2de5c546c3e38f36676c7e22dd040e5b540fc258f72194e7ae17af3f2bf7f0b5'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='9e376a3f2c9a3dc5394fc2f3da480f72b9103c3b71d39d041dc6b08bb65e5724'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 01 May 2021 03:39:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:401a42e1eb4fe87d89990847d6ef97767b5ac57457c8001203ee2ea137736907`  
		Last Modified: Wed, 17 Mar 2021 00:22:34 GMT  
		Size: 48.3 MB (48263709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f752366003eed4ac964ebb4be3453e3f19d854828f4f50ff708900bb4c42924`  
		Last Modified: Wed, 17 Mar 2021 00:45:21 GMT  
		Size: 15.4 MB (15429957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8bcda41a362d9d88a0d441aea2a331902ccebe904d836ec7c39262478cd3b1`  
		Last Modified: Sat, 01 May 2021 03:45:17 GMT  
		Size: 186.0 MB (186003808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:5461fcc71b08f2bd313a4bbb389870e2eb0f6071d83aeb37293a8909248350c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.4 MB (247429176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0036efabdbea8a7f417f80878edb632149151c2069e41b272a011b18b9119ba`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 01 May 2021 02:34:14 GMT
ADD file:f71ab8aa2d773f52af43dee8a58345e3c64f23cf6dc9722fc2116449655ca0ce in / 
# Sat, 01 May 2021 02:34:16 GMT
CMD ["/bin/bash"]
# Sat, 01 May 2021 02:59:26 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Sat, 01 May 2021 02:59:27 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Sat, 01 May 2021 02:59:28 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 May 2021 02:59:30 GMT
ENV LANG=en_US.UTF-8
# Sat, 01 May 2021 02:59:31 GMT
ENV JAVA_VERSION=17-ea+20
# Sat, 01 May 2021 02:59:57 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='2de5c546c3e38f36676c7e22dd040e5b540fc258f72194e7ae17af3f2bf7f0b5'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='9e376a3f2c9a3dc5394fc2f3da480f72b9103c3b71d39d041dc6b08bb65e5724'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 01 May 2021 03:00:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:dbfc55cb74dd07b793cdc9b4bc835fcfdb6091dad8e24cd2a6fe84ec70a2c3a6`  
		Last Modified: Sat, 01 May 2021 02:35:18 GMT  
		Size: 48.9 MB (48874038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0431cdcee2306a17be0ad5fd6791cd432218c8671e4eb75ea3a708d15ef0c6c4`  
		Last Modified: Sat, 01 May 2021 03:07:27 GMT  
		Size: 16.5 MB (16472881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00db1c3eff71fe0b027665184cd9d3970c6d0948258c0b9b99aae77a404539e`  
		Last Modified: Sat, 01 May 2021 03:07:50 GMT  
		Size: 182.1 MB (182082257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
