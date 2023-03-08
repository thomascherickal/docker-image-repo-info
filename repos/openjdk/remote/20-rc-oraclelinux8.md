## `openjdk:20-rc-oraclelinux8`

```console
$ docker pull openjdk@sha256:a7fc0189c1fb26d3c98efc4f66120d898e9f4d08c832d5d5b28adde3a14f3d93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-rc-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:f0a8345f95d44036be5a6b658e4a0e675204a3b27b4ad68e436824b24a9f36dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.7 MB (257698173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90688df26b6515d46dbc2d335a11ad038110795cdd57c8eb8b39b2da72483f25`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:31 GMT
ADD file:eca2b657866c594c67fc9041ad2a4a309e62fc8338add46c3917517649f748b2 in / 
# Wed, 08 Mar 2023 20:22:32 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:53:15 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 08 Mar 2023 20:54:53 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 08 Mar 2023 20:54:53 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 20:54:54 GMT
ENV LANG=C.UTF-8
# Wed, 08 Mar 2023 20:54:54 GMT
ENV JAVA_VERSION=20
# Wed, 08 Mar 2023 20:55:04 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-x64_bin.tar.gz'; 			downloadSha256='bb863b2d542976d1ae4b7b81af3e78b1e4247a64644350b552d298d8dc5980dc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-aarch64_bin.tar.gz'; 			downloadSha256='b671dd1513e7bd4f3de6b1424a90a4998997a67593bf259936d55f5e83e31959'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 08 Mar 2023 20:55:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:767a87c583278931a33db59dc8586fdcfa03c53a801cce573f0e861c31ec4c89`  
		Last Modified: Wed, 08 Mar 2023 20:24:06 GMT  
		Size: 44.6 MB (44557814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754d31dea44245a0029d262dade1fe4e14228c7182d3efde4994c6a76398bc7`  
		Last Modified: Wed, 08 Mar 2023 20:56:42 GMT  
		Size: 15.0 MB (15014167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90192eef3b0c096f280e178c1d1accc0b7c3191bd1a115121a03740b1134b95e`  
		Last Modified: Wed, 08 Mar 2023 20:58:22 GMT  
		Size: 198.1 MB (198126192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-rc-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c46cc372084e55b20d5d8bf02859ce96f188c90ed907a8c1fb9c23613b9a4ff3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255918182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc872572761dc916300761497ddfc56f9ea7a0ff21fef45aea4f9dd10a5b40d9`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:19 GMT
ADD file:18f4bd510f88f32e538884e4e633449c2c8dbf8a5f88b6b6b165ab05872d9507 in / 
# Wed, 08 Mar 2023 21:02:19 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:19:53 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 08 Mar 2023 21:20:56 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 08 Mar 2023 21:20:56 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 21:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 08 Mar 2023 21:20:56 GMT
ENV JAVA_VERSION=20
# Wed, 08 Mar 2023 21:21:07 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-x64_bin.tar.gz'; 			downloadSha256='bb863b2d542976d1ae4b7b81af3e78b1e4247a64644350b552d298d8dc5980dc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-aarch64_bin.tar.gz'; 			downloadSha256='b671dd1513e7bd4f3de6b1424a90a4998997a67593bf259936d55f5e83e31959'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 08 Mar 2023 21:21:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8ff0c9d62930fe3f55e00ba3be2db6be3643b07da9804d1c9b83b0d3181f0df5`  
		Last Modified: Wed, 08 Mar 2023 21:03:40 GMT  
		Size: 43.5 MB (43456139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec39ece690c19b75d657ca26bf156e883914c8bea4948e081819aff289dc43c5`  
		Last Modified: Wed, 08 Mar 2023 21:22:51 GMT  
		Size: 15.8 MB (15834481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70aa63464eb39b4f530bfef9e20ae6f52eadc144ace349fe8701455bdd9bc8bf`  
		Last Modified: Wed, 08 Mar 2023 21:24:25 GMT  
		Size: 196.6 MB (196627562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
