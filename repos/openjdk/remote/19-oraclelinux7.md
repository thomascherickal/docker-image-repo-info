## `openjdk:19-oraclelinux7`

```console
$ docker pull openjdk@sha256:6fab07c10f776aa2353aa40206e4f694190d5117e5016e2be2cf6dd40dd73cb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:c2341e80b2a3a3fb1b78cd3c4142c9872810af53b833a96c528b95785360fc13
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.9 MB (253874936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9783333f0258e39de00b3a208cf726218fd11f0a921a0f35c69661ecdc433736`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 12 Jan 2022 22:34:30 GMT
ADD file:18acb1f3ef1ffe1aeaff1aa22861026180d22104f6f14dd8bc4656777800fd9f in / 
# Wed, 12 Jan 2022 22:34:30 GMT
CMD ["/bin/bash"]
# Wed, 12 Jan 2022 22:51:37 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 12 Jan 2022 22:51:37 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Wed, 12 Jan 2022 22:51:38 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Jan 2022 22:51:38 GMT
ENV LANG=en_US.UTF-8
# Fri, 11 Feb 2022 23:49:47 GMT
ENV JAVA_VERSION=19-ea+9
# Fri, 11 Feb 2022 23:49:58 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/9/GPL/openjdk-19-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='df0cd18dd2885e213244d96e894df4b7f4570eec80a3110f3e50663ba3019c36'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/9/GPL/openjdk-19-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='a77a19b7ec6cd8b57ed1d35d893b166b3d2d5e60036d559fd71f37733bf08031'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:49:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1e1d49338f200e5dab7ef55f9d3a37259af48812603e07ae59e43615f9038b27`  
		Last Modified: Wed, 12 Jan 2022 22:35:18 GMT  
		Size: 48.3 MB (48330956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c20bdba8622bf1a49d6c3edad81bd7ef39ec5a507eb70d2e536a70e60263ba4`  
		Last Modified: Wed, 12 Jan 2022 23:00:42 GMT  
		Size: 15.4 MB (15388577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad735d4a5bde6b295c6c17737af3db08ffc888dc89027f550677140a14a97a`  
		Last Modified: Sat, 12 Feb 2022 00:11:34 GMT  
		Size: 190.2 MB (190155403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:050ebefbf023c2ec1a04c2d4e0d833b4483bafd4ca7859a80c41263191b3b731
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.6 MB (254573017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9a0a1b35de9e4ebc1afbfc1da1a29683422bca2b22124576427be65996884c5`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 12 Jan 2022 21:41:07 GMT
ADD file:64aef77ed2e10e924b07f118b92f579949f920597f01ce3580c3cd17fc289b87 in / 
# Wed, 12 Jan 2022 21:41:08 GMT
CMD ["/bin/bash"]
# Wed, 12 Jan 2022 21:58:19 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 12 Jan 2022 21:58:20 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Wed, 12 Jan 2022 21:58:21 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Jan 2022 21:58:22 GMT
ENV LANG=en_US.UTF-8
# Sat, 12 Feb 2022 00:06:56 GMT
ENV JAVA_VERSION=19-ea+9
# Sat, 12 Feb 2022 00:07:16 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/9/GPL/openjdk-19-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='df0cd18dd2885e213244d96e894df4b7f4570eec80a3110f3e50663ba3019c36'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/9/GPL/openjdk-19-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='a77a19b7ec6cd8b57ed1d35d893b166b3d2d5e60036d559fd71f37733bf08031'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:07:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:89ad662320eff0a72aa4fc7f7af6e2a2ffe2dc642aacc7fcf25ada107b2cc3de`  
		Last Modified: Wed, 12 Jan 2022 21:42:00 GMT  
		Size: 48.9 MB (48902767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcbd5e1a30531d664d4f4f1f2c5a28be251ea96d8b492a51eabd8b7339c2f97`  
		Last Modified: Wed, 12 Jan 2022 22:12:56 GMT  
		Size: 16.5 MB (16464202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c040d54017a3ad27d6458983c16eacd388a1f3a62ba75e794f6fe10dd0843b8`  
		Last Modified: Sat, 12 Feb 2022 00:29:22 GMT  
		Size: 189.2 MB (189206048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
