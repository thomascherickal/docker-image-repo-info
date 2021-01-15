## `openjdk:16-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:4815c5f44d27d80a4113538c8b77afacfff357ee142824b48f8f7884925f27ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:e2f47c47c75a0838e4901bce333f5a0b87bf58c32d5c9879b3bb9757abf4b9a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.5 MB (248533450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71175fd9c78e6deda42b73341d15bfa6cdff9ff92eb7327a71601627c66f453c`
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
# Fri, 15 Jan 2021 01:00:05 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 15 Jan 2021 01:00:06 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Jan 2021 01:00:06 GMT
ENV JAVA_VERSION=16-ea+31
# Fri, 15 Jan 2021 01:00:22 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/31/GPL/openjdk-16-ea+31_linux-aarch64_bin.tar.gz; 			downloadSha256=619122347e25dccbc419168329b659cdb1967570431bc09f597a791107484554; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/31/GPL/openjdk-16-ea+31_linux-x64_bin.tar.gz; 			downloadSha256=f43aa41b3c71b9e278a37fd33a94579a8039e07abd21841ad9e1e0a4582abf24; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 15 Jan 2021 01:00:22 GMT
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
	-	`sha256:3829aca4c13532f300542bc73fdb3794a38c0db5f348185735603731596a833b`  
		Last Modified: Fri, 15 Jan 2021 01:11:00 GMT  
		Size: 184.8 MB (184840953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c4b233b6e39deb833fdfa5ecfcc2f8772f3dd5cf34c7cc4ccd039edc8fbd15e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.5 MB (244465775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fafe20eadd8980cebe0af6132266dd1380c163d0231e99874eee0511205de44f`
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
# Fri, 15 Jan 2021 00:47:58 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 15 Jan 2021 00:47:59 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Jan 2021 22:49:22 GMT
ENV JAVA_VERSION=16-ea+32
# Fri, 15 Jan 2021 22:49:45 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/32/GPL/openjdk-16-ea+32_linux-aarch64_bin.tar.gz; 			downloadSha256=c4ccb6df63b7b973504ad4dec0164d308d5dce7a5e2dcc508180deda33d4e61a; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/32/GPL/openjdk-16-ea+32_linux-x64_bin.tar.gz; 			downloadSha256=c951c0f2d55bc67fecbe0913675811721d13de16f4a81bf5363b660d17c02f0b; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 15 Jan 2021 22:49:47 GMT
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
	-	`sha256:ded29f8c6917694a946c246d03faf5215807ca506e02c22a95d66dff4529ed86`  
		Last Modified: Fri, 15 Jan 2021 23:00:10 GMT  
		Size: 179.1 MB (179136751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
