## `openjdk:21-ea-19-oraclelinux7`

```console
$ docker pull openjdk@sha256:22a1efcaf2609c8bf2176a7c0dd38071b089b7778cd26289cf2d36d6a8610ece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-19-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:4d8c8b80c1cf2a4ec418fe18cbf64695eedd65c5993218ba32002c737de4f04e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266317069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55c6106945bbb6c00af725a468d56a360fb4d5503e73cc0fef7e36323ee9624f`
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
# Fri, 21 Apr 2023 20:07:20 GMT
ENV JAVA_VERSION=21-ea+19
# Fri, 21 Apr 2023 20:07:29 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5af95497753fbc33981f5ab1267fbd3be57e4095ceca9806490a25b56f819007'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='d08fe17feea7fa18c4e9ee9918496974d0194d1fac9a485d47cc2d30601c3682'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Apr 2023 20:07:30 GMT
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
	-	`sha256:f4dc6073e1a67503bb2fa89c04b501c4f3f4eeb73a838b41d219304a93a164d1`  
		Last Modified: Fri, 21 Apr 2023 20:10:01 GMT  
		Size: 201.6 MB (201580309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-19-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:319016a0dd363f19ec9a7e9d9237a0eb6a58ddccc0bbb9661dc59104d09687fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266236076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3105692971b069d3caf13c989639f740cca600918862ffba8c815dee2a681db3`
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
# Fri, 21 Apr 2023 20:22:38 GMT
ENV JAVA_VERSION=21-ea+19
# Fri, 21 Apr 2023 20:22:51 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5af95497753fbc33981f5ab1267fbd3be57e4095ceca9806490a25b56f819007'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='d08fe17feea7fa18c4e9ee9918496974d0194d1fac9a485d47cc2d30601c3682'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Apr 2023 20:22:53 GMT
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
	-	`sha256:b7494de766935568d19c707bcb61576a157908444b3abf7b304e902e0f05ba9e`  
		Last Modified: Fri, 21 Apr 2023 20:25:09 GMT  
		Size: 199.9 MB (199943271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
