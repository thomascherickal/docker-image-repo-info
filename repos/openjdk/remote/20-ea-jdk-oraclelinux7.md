## `openjdk:20-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:9bd22fc7ad38e91e8cb764c019d406c9d33979ec8db079fd906d19f49389e3e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:01b75efaa6d677bfcca1449d2ad7ca9bc337f1e81110324b1ef6095d511b86fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.1 MB (260136524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc238f8bf87b7cc8be6f9fabfc72a9f0f7a235dc172ba63e81e8a4745b235826`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 Aug 2022 19:35:42 GMT
ADD file:adf7ebc1d65494dba22f4f0a12f2f8f63128836b87646ffd6e9964f936343e6d in / 
# Wed, 24 Aug 2022 19:35:43 GMT
CMD ["/bin/bash"]
# Wed, 24 Aug 2022 22:44:32 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 24 Aug 2022 22:44:32 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 24 Aug 2022 22:44:32 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 22:44:33 GMT
ENV LANG=en_US.UTF-8
# Thu, 01 Sep 2022 23:29:17 GMT
ENV JAVA_VERSION=20-ea+13
# Thu, 01 Sep 2022 23:29:27 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/13/GPL/openjdk-20-ea+13_linux-x64_bin.tar.gz'; 			downloadSha256='93758735b85b0f9e8a98728ad636942bcf266476824286754fe6dbd2a2f6aeff'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/13/GPL/openjdk-20-ea+13_linux-aarch64_bin.tar.gz'; 			downloadSha256='305cd60ab947992620abe377f9d1fe876c6a80db3fab369a8cb5517edbfc30be'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 01 Sep 2022 23:29:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9815334b7810943f0c417fa41a2732d56b098252185c5749c2c2ce80f8e8e140`  
		Last Modified: Wed, 24 Aug 2022 19:37:41 GMT  
		Size: 48.7 MB (48727120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbb6577271d2ea4eb7961ad553fcac407890cd27f6514b5d071119191d585fd`  
		Last Modified: Wed, 24 Aug 2022 22:49:44 GMT  
		Size: 14.2 MB (14230815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654474eccfb39b4e3988e065256412ac8367c049a203f986dd4028a74f321a1e`  
		Last Modified: Thu, 01 Sep 2022 23:35:07 GMT  
		Size: 197.2 MB (197178589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:730e884dd4017d393da168411a49d5feecb5a619aa30c1b7ac689f7d872352c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.3 MB (260299999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a82e785a99ae59ce0a76782740269497935632c690e89993b75203bec0fe40`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 Aug 2022 19:55:21 GMT
ADD file:58b53a780a05a9f314e6821fd85f38a0d86fed5a98ab7c3fd52b0ea2341c3d64 in / 
# Wed, 24 Aug 2022 19:55:22 GMT
CMD ["/bin/bash"]
# Wed, 24 Aug 2022 23:31:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 24 Aug 2022 23:31:54 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 24 Aug 2022 23:31:55 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 23:31:56 GMT
ENV LANG=en_US.UTF-8
# Fri, 02 Sep 2022 00:43:07 GMT
ENV JAVA_VERSION=20-ea+13
# Fri, 02 Sep 2022 00:43:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/13/GPL/openjdk-20-ea+13_linux-x64_bin.tar.gz'; 			downloadSha256='93758735b85b0f9e8a98728ad636942bcf266476824286754fe6dbd2a2f6aeff'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/13/GPL/openjdk-20-ea+13_linux-aarch64_bin.tar.gz'; 			downloadSha256='305cd60ab947992620abe377f9d1fe876c6a80db3fab369a8cb5517edbfc30be'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 02 Sep 2022 00:43:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9d094a37c2b34cb4c876f39d579c422eba5a195ec17dff5a5fcbbbd9398dafef`  
		Last Modified: Wed, 24 Aug 2022 19:57:30 GMT  
		Size: 49.3 MB (49309770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346cd8d935004b602845ed18ab7ddf7b6bf15cfcb9eb50d1b98f6153c188f3a3`  
		Last Modified: Wed, 24 Aug 2022 23:41:46 GMT  
		Size: 15.3 MB (15266557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a64b3f4382a3bc4fe30566b25acfb2b95b7be652b90dda9ad36ee3f1b879f1c`  
		Last Modified: Fri, 02 Sep 2022 00:52:30 GMT  
		Size: 195.7 MB (195723672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
