## `openjdk:21-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:9c4b283614fd857a5f9a33a9a0dbbbd505afa042fd6828bb8904fb4c06ef8b76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:874d487a3b565483366d1105e131444c52cfe7ffbfd4dfca74d39ab6c4eb6be3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.1 MB (264118712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44472ec3c8e8086f5258ff97b63963fb4a61c4c4b10bea8347cfce1765aaf5b7`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:54 GMT
ADD file:e205deb729daf99a168c27d3f97cd2b69e736fc9d4bee9ea220ec86921574a0f in / 
# Wed, 08 Mar 2023 20:22:55 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:54:26 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 08 Mar 2023 20:54:26 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 08 Mar 2023 20:54:26 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 20:54:26 GMT
ENV LANG=en_US.UTF-8
# Wed, 08 Mar 2023 20:54:27 GMT
ENV JAVA_VERSION=21-ea+12
# Wed, 08 Mar 2023 20:54:37 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/12/GPL/openjdk-21-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='da247094c9b9e7b4ab18b5e36adc89e3b7f6ee77192816ce059b933e23e09fca'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/12/GPL/openjdk-21-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='ea0bf5244a8b27f1c111cb40cb161186c9217f0bbc31e3a019b81c21505c8f18'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 08 Mar 2023 20:54:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7b659169cb9226d08443358aa4e8147f3144614ac33f7a41217b0cf62a4d3326`  
		Last Modified: Wed, 08 Mar 2023 20:24:41 GMT  
		Size: 50.5 MB (50467964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efc12c70e0ba49ea5eb742d598c3d36a33b4d7407f8be1a8ac8641ad14e0a56`  
		Last Modified: Wed, 08 Mar 2023 20:57:27 GMT  
		Size: 14.2 MB (14236997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1ebb1016615c3dd11745c5b2b1ead20f7c409ecb9fb6115f8e6f4a28221027`  
		Last Modified: Wed, 08 Mar 2023 20:57:40 GMT  
		Size: 199.4 MB (199413751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f7609cdb241ced9435704764f510eb764b86060afecf4e7b2280f5c920b5a474
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.2 MB (264173894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01b81ec8590d9e7740e6c87718b20c45e5fc7e6e368520c9013bbed49645108`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:36 GMT
ADD file:d11a3555d107d9db5ab5621675aa2ecf27ec872cc591769bdc75129ff602dfd7 in / 
# Wed, 08 Mar 2023 21:02:37 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:20:32 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 08 Mar 2023 21:20:32 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 08 Mar 2023 21:20:32 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 21:20:32 GMT
ENV LANG=en_US.UTF-8
# Wed, 08 Mar 2023 21:20:32 GMT
ENV JAVA_VERSION=21-ea+12
# Wed, 08 Mar 2023 21:20:44 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/12/GPL/openjdk-21-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='da247094c9b9e7b4ab18b5e36adc89e3b7f6ee77192816ce059b933e23e09fca'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/12/GPL/openjdk-21-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='ea0bf5244a8b27f1c111cb40cb161186c9217f0bbc31e3a019b81c21505c8f18'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 08 Mar 2023 21:20:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4b689a883b146569199f6bfaadce974725d68f1cd14d01950efe476637febe12`  
		Last Modified: Wed, 08 Mar 2023 21:04:11 GMT  
		Size: 51.0 MB (51027010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ce6fa2927eee2bba1cdfc5060760f859a7073e02bf271b9b61999943c2211d`  
		Last Modified: Wed, 08 Mar 2023 21:23:34 GMT  
		Size: 15.2 MB (15249325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f150fae5e3bbb98005499c5999f5a682b178adaf9a28ad7ff6cf863cf4d90c`  
		Last Modified: Wed, 08 Mar 2023 21:23:44 GMT  
		Size: 197.9 MB (197897559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
