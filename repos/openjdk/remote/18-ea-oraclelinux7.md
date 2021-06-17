## `openjdk:18-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:62917d79100b9b1d690de593bd77fbbfc538067419bebb3d2b1beb677eaf0269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:ab65dce1e11cc221eabf150b958bd31b87c2dfbb222c3872fe79bf9171d4fca2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.7 MB (251656423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:304d8063cb5b85648d7322235c32d1aaaa00507ba8495fa3c6a5ff6c37b41e25`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 17 Jun 2021 16:51:20 GMT
ADD file:46efe0cb70a1c4f574c3b3e1fb9b9733930d246bb8077c4ec2160a840697e6c8 in / 
# Thu, 17 Jun 2021 16:51:21 GMT
CMD ["/bin/bash"]
# Thu, 17 Jun 2021 17:08:18 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 17 Jun 2021 17:08:19 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 17 Jun 2021 17:08:19 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Jun 2021 17:08:19 GMT
ENV LANG=en_US.UTF-8
# Thu, 17 Jun 2021 17:08:19 GMT
ENV JAVA_VERSION=18-ea+1
# Thu, 17 Jun 2021 17:08:30 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/1/GPL/openjdk-18-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='277c0021c542fbda35d2643351148fa6cceac66b5beca24016c75fafeed815de'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/1/GPL/openjdk-18-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='6b615e986bc649e30072f1a7e88986e7a55cad95756c982a2f02f278ec8fe05c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Jun 2021 17:08:31 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7627bfb99533146fcb8374f557bc24c36505fb2ee8578ec6072a821200247bbb`  
		Last Modified: Thu, 17 Jun 2021 16:52:21 GMT  
		Size: 48.3 MB (48260810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb70fb8946cabfaff2f43cee5915a69ad662b0294e9c91d8f545898e92ed32fd`  
		Last Modified: Thu, 17 Jun 2021 17:14:39 GMT  
		Size: 15.4 MB (15426613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e70709f380d03b1358e661e5ad994d974bfbb47a2d10c392eaf191dc587aef1`  
		Last Modified: Thu, 17 Jun 2021 17:14:51 GMT  
		Size: 188.0 MB (187969000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:275bade2a1539a4e23a60d625f3f4cc1fd0ed40674d5c5a917ba91a0fb938fc8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.1 MB (252060170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9041e7cc28f73172c770ceb9bbd89a1e5ee016a0b67ef98fe3fe060a5b71a283`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 17 Jun 2021 16:51:08 GMT
ADD file:256f7e1c19fbbacd7c7650e1e9991f3617703ba349f259624d78e4393e945665 in / 
# Thu, 17 Jun 2021 16:51:08 GMT
CMD ["/bin/bash"]
# Thu, 17 Jun 2021 17:08:43 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 17 Jun 2021 17:08:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 17 Jun 2021 17:08:43 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Jun 2021 17:08:43 GMT
ENV LANG=en_US.UTF-8
# Thu, 17 Jun 2021 17:08:43 GMT
ENV JAVA_VERSION=18-ea+1
# Thu, 17 Jun 2021 17:09:17 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/1/GPL/openjdk-18-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='277c0021c542fbda35d2643351148fa6cceac66b5beca24016c75fafeed815de'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/1/GPL/openjdk-18-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='6b615e986bc649e30072f1a7e88986e7a55cad95756c982a2f02f278ec8fe05c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Jun 2021 17:09:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9a3d615f016c21e1c5fef521352cdd990a61abfd09a26d7124c61e33b2cab56a`  
		Last Modified: Thu, 17 Jun 2021 16:52:10 GMT  
		Size: 48.9 MB (48858581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a33d75d2c35cdf1c0dc42b99124399c0375b12141be4bddb4b819732453cb`  
		Last Modified: Thu, 17 Jun 2021 17:23:33 GMT  
		Size: 16.4 MB (16419706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405ef90c82df2e1ef6f23143719008d812497b4b2c11f0600332c6e4268f2672`  
		Last Modified: Thu, 17 Jun 2021 17:23:48 GMT  
		Size: 186.8 MB (186781883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
