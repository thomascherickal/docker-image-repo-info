## `openjdk:19-ea-23-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:11039f3aea46590dc6d0a9eef042d8a3fa4345bae843ab179bb408f642d04386
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:19-ea-23-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:95f9f3766f4bdf10be4ec03f4758cf27b76706583c5d02c8f48e15bb43014503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.1 MB (259148714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a09f1c86bd1eced7e89dc9290989986cc6adbe8eb84c7bfb32b9a58302624699`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 19 May 2022 17:55:42 GMT
ADD file:3d80a0730bc69825f18f411b67d8e8a6eb5b2450223ab171cf3f4f7f8b43d021 in / 
# Thu, 19 May 2022 17:55:44 GMT
CMD ["/bin/bash"]
# Thu, 19 May 2022 19:04:26 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 19 May 2022 19:04:27 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 19 May 2022 19:04:28 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 May 2022 19:04:29 GMT
ENV LANG=en_US.UTF-8
# Fri, 20 May 2022 21:03:53 GMT
ENV JAVA_VERSION=19-ea+23
# Fri, 20 May 2022 21:04:11 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/23/GPL/openjdk-19-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='37187e2eecb64237757cf5d5b2c7a94b25d2b03f3ea5b12bf77a5fe8b1508ac4'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/23/GPL/openjdk-19-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad7e6c255a6a0fcb02b05a879036c1d3029693c577b7cc97323f7e43901e48e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 20 May 2022 21:04:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9932f90ce40726b220e1a83ec69eaecb5ceec5409d33a736f6189de512eac36e`  
		Last Modified: Thu, 19 May 2022 17:56:42 GMT  
		Size: 49.3 MB (49337178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aa262ef1f7aae5da5cd2e580c02388ffbd2dc26b81fb14478c79b9074c22a3`  
		Last Modified: Thu, 19 May 2022 19:16:45 GMT  
		Size: 15.3 MB (15268963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc9cdcdf29c1c8ad9b1ab0d0f8d839555c4cf6895f17725a0717f7ce7fec913`  
		Last Modified: Fri, 20 May 2022 21:17:23 GMT  
		Size: 194.5 MB (194542573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
