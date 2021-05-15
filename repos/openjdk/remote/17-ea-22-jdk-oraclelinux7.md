## `openjdk:17-ea-22-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:b4eb5d379e26835842752516b933e8c504ae38bab9b62753fc509f7ea36c27ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-ea-22-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:9c1ec05e56e3e6b8854edd31962433a256779941df172db41f60c19957a17c2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.7 MB (249709558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21db2a1d91867922c30a421b5152efed43169b0d8b692df665134ef4cdabded2`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 06 May 2021 00:10:37 GMT
ADD file:7532c4c6850a2e95d341f39828f60573728d50ba1fc6264ed19bb36eb4b24d1c in / 
# Thu, 06 May 2021 00:10:37 GMT
CMD ["/bin/bash"]
# Thu, 06 May 2021 00:27:43 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 06 May 2021 00:27:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Thu, 06 May 2021 00:27:43 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 00:27:43 GMT
ENV LANG=en_US.UTF-8
# Fri, 14 May 2021 19:27:22 GMT
ENV JAVA_VERSION=17-ea+22
# Fri, 14 May 2021 19:27:38 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/22/GPL/openjdk-17-ea+22_linux-x64_bin.tar.gz'; 			downloadSha256='68cbe678787e56de88967003071f05b47eb5cd3bbb1dd083f23bf4b8f23b25c9'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/22/GPL/openjdk-17-ea+22_linux-aarch64_bin.tar.gz'; 			downloadSha256='fef8858675921c49b693311954fd593ec8414e00609e96c1f6262ca8c9801a0c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 14 May 2021 19:27:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:22f7711cf64307564c3293688489295d9458bac2ca47cd6576382cfb75c9d2b9`  
		Last Modified: Thu, 06 May 2021 00:11:49 GMT  
		Size: 48.3 MB (48258661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87180291cc45c5c610f6909495ba989b36ef14701a331d8689e264f9d7c23796`  
		Last Modified: Thu, 06 May 2021 00:32:56 GMT  
		Size: 15.4 MB (15423518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d513a8c41d5bcc2d8d72106ce80b2bf9a5cc4d7d560b36e05725970336a688ba`  
		Last Modified: Fri, 14 May 2021 19:33:21 GMT  
		Size: 186.0 MB (186027379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-22-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:d3f836221e22e8d58dd7c3b531ce13df507e4e00097bd8c88cbe82a42d2dd792
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.4 MB (247440824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd38a4ce49f7f4fd8371f4e3e520d07daa470285efeb9a7ee8dd591377efde1`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 06 May 2021 00:13:32 GMT
ADD file:57303578fa11d312dcc51eb7aef116316c2b60e48b533a1471e2f2ba915ee46a in / 
# Thu, 06 May 2021 00:13:35 GMT
CMD ["/bin/bash"]
# Thu, 06 May 2021 00:32:13 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 06 May 2021 00:32:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Thu, 06 May 2021 00:32:15 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 00:32:16 GMT
ENV LANG=en_US.UTF-8
# Fri, 14 May 2021 19:50:33 GMT
ENV JAVA_VERSION=17-ea+22
# Fri, 14 May 2021 19:51:07 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/22/GPL/openjdk-17-ea+22_linux-x64_bin.tar.gz'; 			downloadSha256='68cbe678787e56de88967003071f05b47eb5cd3bbb1dd083f23bf4b8f23b25c9'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/22/GPL/openjdk-17-ea+22_linux-aarch64_bin.tar.gz'; 			downloadSha256='fef8858675921c49b693311954fd593ec8414e00609e96c1f6262ca8c9801a0c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 14 May 2021 19:51:10 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6d575bf1166e11ab792c567b7bdfab507a987976bc375994e3516987e6e1e600`  
		Last Modified: Thu, 06 May 2021 00:14:38 GMT  
		Size: 48.9 MB (48869643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892e1551bf2c1decd5f1f367d2f9dbf15317e29aa12b267cf59b9c255a91b34`  
		Last Modified: Thu, 06 May 2021 00:39:13 GMT  
		Size: 16.5 MB (16472243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e017a879982bbcd058b05696808ffd4747191957d7d5249307ac294de0cf15b0`  
		Last Modified: Fri, 14 May 2021 19:57:21 GMT  
		Size: 182.1 MB (182098938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
