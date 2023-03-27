## `openjdk:21-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:51f4785e273ed5e4474d5906bc7c11ecbfda4f47dd640e25902531470604b62d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:479fce92de0f78c796aaeb64e103baf615d2e61184d49cbe0e956ea21033ebb6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266164993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7bb4edf9bc684fb0858dc0e8a36e3985656dd647f794ebddb938144f37512b8`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Mar 2023 19:26:42 GMT
ADD file:c2562ae661b3cd914b2c0dd27aba7ee36bffbeb92415b7b80c111a5d563d07ed in / 
# Tue, 21 Mar 2023 19:26:43 GMT
CMD ["/bin/bash"]
# Tue, 21 Mar 2023 20:47:46 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 21 Mar 2023 20:47:46 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Tue, 21 Mar 2023 20:47:46 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Mar 2023 20:47:46 GMT
ENV LANG=en_US.UTF-8
# Tue, 21 Mar 2023 20:47:47 GMT
ENV JAVA_VERSION=21-ea+14
# Tue, 21 Mar 2023 20:47:56 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/14/GPL/openjdk-21-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='5ff9e95f12627e7f9c4b2e61d4ddfa5eb224f6106eff7620a487244be71d9787'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/14/GPL/openjdk-21-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='32b9ef0cafec4114aac8917e9ad754c7a3bdcfbc47143e4e5182757a0311ae66'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 21 Mar 2023 20:47:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2ec521688c56b41126476e7ab1f7ab7305384f5b5326e80a8ba52b8d4deead22`  
		Last Modified: Tue, 21 Mar 2023 19:27:26 GMT  
		Size: 50.5 MB (50471128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea283652a57d33ca137043965b4c70fa3e5d30b9487b344159545deda829f9b`  
		Last Modified: Tue, 21 Mar 2023 20:49:09 GMT  
		Size: 14.3 MB (14252036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b984e7880638e9a4d1dbcc94e4f7cf9b1d3353f5630923e8034099b2a7dd5ed`  
		Last Modified: Tue, 21 Mar 2023 20:49:22 GMT  
		Size: 201.4 MB (201441829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:80b6cc788f96b50874b7f80d495234b2893e463bde42193c44f868089c2c7665
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266311016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97cb3e920bad16f5ceba76cc0d72adb51bfa62745b8a9ed2ec56dbdd03e8bc08`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Mar 2023 19:44:52 GMT
ADD file:a9428dda3ec7ae554537bb583832aa2d30484c863bf95c68e460df5858c4c0bf in / 
# Tue, 21 Mar 2023 19:44:53 GMT
CMD ["/bin/bash"]
# Tue, 21 Mar 2023 21:03:26 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 21 Mar 2023 21:03:26 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Tue, 21 Mar 2023 21:03:26 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Mar 2023 21:03:27 GMT
ENV LANG=en_US.UTF-8
# Mon, 27 Mar 2023 22:47:33 GMT
ENV JAVA_VERSION=21-ea+15
# Mon, 27 Mar 2023 22:47:46 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/15/GPL/openjdk-21-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='0fec1002b8c8975b181bd6966a817028d6b373cbc759254231f9b96db1fe6edd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/15/GPL/openjdk-21-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='93cc1eb6202093a127f1f9ed2e866a51dff29321f878085c18f317cefb113ffc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 27 Mar 2023 22:47:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:41dbc375a859f3e982b6147e2fd05b413e6995b4b728c27f1b851f64a31c004c`  
		Last Modified: Tue, 21 Mar 2023 19:45:30 GMT  
		Size: 51.0 MB (51027591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7ddfee215622f57465bb8dace7332092902d9c16c5bfa61ec64821d8cbb5c`  
		Last Modified: Tue, 21 Mar 2023 21:04:45 GMT  
		Size: 15.2 MB (15249122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70aceb63bb2c892c80155ec624c331102d707c733bcfc8d4bde9260f31a3984`  
		Last Modified: Mon, 27 Mar 2023 22:50:03 GMT  
		Size: 200.0 MB (200034303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
