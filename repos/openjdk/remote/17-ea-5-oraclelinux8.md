## `openjdk:17-ea-5-oraclelinux8`

```console
$ docker pull openjdk@sha256:99169dbd9707ac68ba7235f893a1eeeb06869171a7c3a5e96b6aa1d52c4e4add
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `openjdk:17-ea-5-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:270b9d5f823e4217358578f4b9fe5ae96fbe7f3876c886b39a7bf0d993079187
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.3 MB (236290266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b09e2e7ee839ef8f1981df6157b189c3f4b0d31d9af912931223870db48d3168`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 15 Jan 2021 00:05:48 GMT
ADD file:ad2b2ddca8e17229cc8d1380ecda32c4b2c04f1e2aed8f493f745c6352b34e60 in / 
# Fri, 15 Jan 2021 00:05:49 GMT
CMD ["/bin/bash"]
# Fri, 15 Jan 2021 00:43:36 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 15 Jan 2021 00:43:38 GMT
ENV LANG=C.UTF-8
# Fri, 15 Jan 2021 00:43:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 15 Jan 2021 00:43:39 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Jan 2021 22:45:29 GMT
ENV JAVA_VERSION=17-ea+5
# Fri, 15 Jan 2021 22:46:23 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk17/5/GPL/openjdk-17-ea+5_linux-aarch64_bin.tar.gz; 			downloadSha256=5320fe7df7906893dc060984832ade284ffbe9cf767e4428e628cf517b1b0a92; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk17/5/GPL/openjdk-17-ea+5_linux-x64_bin.tar.gz; 			downloadSha256=0de74da4de6dfd013fad9b1c121b58568128117d3e9ac66508b05b46ebbdce1d; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 15 Jan 2021 22:46:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d0eecbd2c3e7306adbf5b4a0d9bebc7d266ebe78bda044d35b0994c1cf655a54`  
		Last Modified: Wed, 06 Jan 2021 20:47:00 GMT  
		Size: 42.0 MB (41996293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8f86f1d6521cdc8416801b8dd0b15d9a5a85bfa3eb8f9afa832aa8cc652732`  
		Last Modified: Fri, 15 Jan 2021 00:55:15 GMT  
		Size: 14.1 MB (14057398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fefd666fb2596b9f1be7a34e9e43dc996f94044dc135255da29f33243067890`  
		Last Modified: Fri, 15 Jan 2021 22:55:44 GMT  
		Size: 180.2 MB (180236575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
