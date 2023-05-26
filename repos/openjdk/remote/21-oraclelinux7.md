## `openjdk:21-oraclelinux7`

```console
$ docker pull openjdk@sha256:0e09a12920b17edfd6220778c546a1d55701981f751c039a47005b48e715fd5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:bcfd8ce6f571cd2ae0ebcae131df37b95668c2094bef69564c35c69f0955f2fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.9 MB (267877142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5779aa8de87d196a2fa26c8b43cdef169e68d889a06e651c32484d2e22a64ab0`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 Mar 2023 22:29:01 GMT
ADD file:a14b5a8b8b6993aeee5ac6052fdf283560d65365e5bcf133ab21c4756439384a in / 
# Fri, 31 Mar 2023 22:29:01 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 23:12:41 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 31 Mar 2023 23:12:42 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 31 Mar 2023 23:12:42 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 31 Mar 2023 23:12:42 GMT
ENV LANG=en_US.UTF-8
# Fri, 26 May 2023 23:05:24 GMT
ENV JAVA_VERSION=21-ea+24
# Fri, 26 May 2023 23:05:34 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='437e740a3ee795a3cf08d6cf5006d03668023151200d5e09ada16d94ef30db22'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='ecabd8a50340461d04d06b8f587bf06c614aed9cb441ee3ff9577e1b10e53035'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 May 2023 23:05:35 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e83e8f2e82cc31391cd0cb4f5ba574ba5eb9708fc0f5dcc34fef53b03ef28f31`  
		Last Modified: Fri, 31 Mar 2023 22:30:40 GMT  
		Size: 50.5 MB (50496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7475b337670740c8f411f4efcbf2d4308101210ec581e69836860ffcd789ca`  
		Last Modified: Fri, 31 Mar 2023 23:14:05 GMT  
		Size: 14.2 MB (14240731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefcdf1a0a831ada1eff224da06dbb6d17fa0e45da28ebfff78324a1637660a0`  
		Last Modified: Fri, 26 May 2023 23:08:12 GMT  
		Size: 203.1 MB (203140382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:60a371707cdc20a32c55a46068c6b1fed2f9339d9fa74b04501ffb420bb1648c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.8 MB (267771754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fc1cddf2c5c79544ed09aa73d3f39bcdafa0cd001379e8e966fe99c113643fb`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 Mar 2023 21:40:35 GMT
ADD file:4fe62bcdc8f181de8e01e791570bbb89f29712a9aef0b329febd817f4fef8887 in / 
# Fri, 31 Mar 2023 21:40:36 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 22:08:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 31 Mar 2023 22:08:06 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 31 Mar 2023 22:08:06 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 31 Mar 2023 22:08:06 GMT
ENV LANG=en_US.UTF-8
# Thu, 25 May 2023 23:40:00 GMT
ENV JAVA_VERSION=21-ea+24
# Thu, 25 May 2023 23:40:13 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='437e740a3ee795a3cf08d6cf5006d03668023151200d5e09ada16d94ef30db22'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='ecabd8a50340461d04d06b8f587bf06c614aed9cb441ee3ff9577e1b10e53035'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 25 May 2023 23:40:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a138fe98397d054834e86c902a0b929bd7cf0261ac671e779f872176569996ab`  
		Last Modified: Fri, 31 Mar 2023 21:42:01 GMT  
		Size: 51.1 MB (51054832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61213d9405aef8db0237e9542508819c698c4d8293ccbd8799a36206032fdd7c`  
		Last Modified: Fri, 31 Mar 2023 22:09:32 GMT  
		Size: 15.2 MB (15237973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8934c25e7373be3d191cf404f435c2ad4fb9aed2eb5a0a74ab1e60c7b75a75`  
		Last Modified: Thu, 25 May 2023 23:42:38 GMT  
		Size: 201.5 MB (201478949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
