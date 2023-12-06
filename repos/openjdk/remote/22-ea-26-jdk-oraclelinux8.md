## `openjdk:22-ea-26-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:191150e69c1f10534adccbdb4b01044686fa36ef8b38db9b84def12ecf5f0af5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-26-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:4b40efd84f2aa9d06a93e2b1240c06b9250ed51af8cfdbd012d36b21d3d7c5fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.5 MB (271487696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23348ef1352e65381388074b9433f86ff4d43e06c8d0e391f52ce2baaf716d83`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 06 Dec 2023 19:23:17 GMT
ADD file:0fefdd26d1656281881908973318cde9ebc07674dc1098bbf40d9ce6acf2f036 in / 
# Wed, 06 Dec 2023 19:23:18 GMT
CMD ["/bin/bash"]
# Wed, 06 Dec 2023 20:00:36 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 06 Dec 2023 20:00:36 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Wed, 06 Dec 2023 20:00:36 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Dec 2023 20:00:36 GMT
ENV LANG=C.UTF-8
# Wed, 06 Dec 2023 20:00:36 GMT
ENV JAVA_VERSION=22-ea+26
# Wed, 06 Dec 2023 20:00:50 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/26/GPL/openjdk-22-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='65f135f44a1f33848f9d8398b7773807cf90eeec08d6ec8e2a9b44d81b7b6d99'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/26/GPL/openjdk-22-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='3933a8d405ab7f0293ecd4351177e731f1eacd1a96ee3f0528b9157940581ce2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 06 Dec 2023 20:00:51 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e9f2695d7e5b00c4289ec17d08776fb4b6664a9c805294c7d5c364b56d3b9435`  
		Last Modified: Wed, 06 Dec 2023 19:24:28 GMT  
		Size: 51.3 MB (51319965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebbf0da9fa600e22c5cd98f435880f2761cb99b69b62426cd495c758cd85ead`  
		Last Modified: Wed, 06 Dec 2023 20:01:37 GMT  
		Size: 15.0 MB (15007096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea9daa735671b25c083594a145bb9a5f8c2c7768049b1a4c463b30418a90f28`  
		Last Modified: Wed, 06 Dec 2023 20:01:50 GMT  
		Size: 205.2 MB (205160635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-26-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:ae9ce2486eefeddafb2fbdc1c571197e25df1f27b7d54a878ba3843209787e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.0 MB (268974216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86781f16893f1d368f21b2b72c4396e8b32d20d91f504a3e0a9b2c5dbea3296f`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Wed, 06 Dec 2023 19:59:22 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 06 Dec 2023 19:59:22 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Wed, 06 Dec 2023 19:59:22 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Dec 2023 19:59:22 GMT
ENV LANG=C.UTF-8
# Wed, 06 Dec 2023 19:59:22 GMT
ENV JAVA_VERSION=22-ea+26
# Wed, 06 Dec 2023 19:59:35 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/26/GPL/openjdk-22-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='65f135f44a1f33848f9d8398b7773807cf90eeec08d6ec8e2a9b44d81b7b6d99'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/26/GPL/openjdk-22-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='3933a8d405ab7f0293ecd4351177e731f1eacd1a96ee3f0528b9157940581ce2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 06 Dec 2023 19:59:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d8c428b27054b71203994f8d4e7663f63c8f02b8d84bad3e34d156fbd7c0b2`  
		Last Modified: Wed, 06 Dec 2023 20:00:26 GMT  
		Size: 15.7 MB (15688463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05481b9b7fa0eb5af731d95c5419908510c4f87965b74fa9480eb150f45114e9`  
		Last Modified: Wed, 06 Dec 2023 20:00:36 GMT  
		Size: 203.2 MB (203213208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
