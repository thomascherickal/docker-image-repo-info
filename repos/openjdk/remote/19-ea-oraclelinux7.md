## `openjdk:19-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:0974e714e8f6d8401bda82e2eeefb65bbbe15b44d718a39a202e5545a4fd22ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:9bc5ad9383d65466243a96fdda20a58f2be740d064f3d55853eed833accdb2b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.9 MB (253921778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46b1b6c037180f6ac93b5a09c9d819f27faac4fa1211471bc3e645eb02c471bd`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Feb 2022 01:15:28 GMT
ADD file:a953cc04974b35909ddbd8826601c0824f8cc920ebc522046d4ca64e69c2c26f in / 
# Thu, 24 Feb 2022 01:15:29 GMT
CMD ["/bin/bash"]
# Thu, 24 Feb 2022 01:47:39 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 24 Feb 2022 01:47:40 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 24 Feb 2022 01:47:40 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Feb 2022 01:47:40 GMT
ENV LANG=en_US.UTF-8
# Thu, 24 Feb 2022 01:47:40 GMT
ENV JAVA_VERSION=19-ea+10
# Thu, 24 Feb 2022 01:48:13 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/10/GPL/openjdk-19-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='21260b7e784c0e74c6730bdbaac70484fde42cf2839b2188dd2c4811d04660d8'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/10/GPL/openjdk-19-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='e41beaf49bdb16dc2eeec5e7e7c535f19444e221daf1cbb97d6e2b7981583156'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 24 Feb 2022 01:48:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5269884ada0dd8683c910050c7cf3a447be8fcb9f733519f759745b117b217cc`  
		Last Modified: Thu, 24 Feb 2022 01:16:17 GMT  
		Size: 48.3 MB (48331243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48833246028b375ed9389617e9b863bfab004c27db95b93b1e8b7c646ce3f9a1`  
		Last Modified: Thu, 24 Feb 2022 01:58:10 GMT  
		Size: 15.4 MB (15402391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7672cb2613e7de3ffdf3872aacd6b01893206f5e16223740cd3f182fcc75a8`  
		Last Modified: Thu, 24 Feb 2022 01:58:23 GMT  
		Size: 190.2 MB (190188144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7cbe42585874c51759950e0187c63752e03163655fbe9a79a61381224f415f85
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.6 MB (254573591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbc054a516d10d5d9826bbc6e7eeab22e0cce79947bb6c8d419657c60c534102`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Feb 2022 01:19:51 GMT
ADD file:c293ee454f68e84cb645f758fa6566a1eb9e75fb5a28101eab9f1cafd97e9226 in / 
# Thu, 24 Feb 2022 01:19:52 GMT
CMD ["/bin/bash"]
# Thu, 24 Feb 2022 02:04:47 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 24 Feb 2022 02:04:47 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 24 Feb 2022 02:04:48 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Feb 2022 02:04:49 GMT
ENV LANG=en_US.UTF-8
# Thu, 24 Feb 2022 02:04:50 GMT
ENV JAVA_VERSION=19-ea+10
# Thu, 24 Feb 2022 02:05:17 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/10/GPL/openjdk-19-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='21260b7e784c0e74c6730bdbaac70484fde42cf2839b2188dd2c4811d04660d8'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/10/GPL/openjdk-19-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='e41beaf49bdb16dc2eeec5e7e7c535f19444e221daf1cbb97d6e2b7981583156'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 24 Feb 2022 02:05:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4402421e0ca8a48b128ce814a1f5f26684df2d5f1caf1afa1ffbb8fabccdf603`  
		Last Modified: Thu, 24 Feb 2022 01:20:47 GMT  
		Size: 48.9 MB (48902111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7e8a0b0254507322b36a7a006c588143e280eb30aeb748e6245570ea648cb7`  
		Last Modified: Thu, 24 Feb 2022 02:21:23 GMT  
		Size: 16.4 MB (16444983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11f056427fd867c1812d4391a3bb983c4a9799f943979de0051301fcc35a217`  
		Last Modified: Thu, 24 Feb 2022 02:21:38 GMT  
		Size: 189.2 MB (189226497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
