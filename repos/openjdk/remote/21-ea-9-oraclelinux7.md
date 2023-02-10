## `openjdk:21-ea-9-oraclelinux7`

```console
$ docker pull openjdk@sha256:ab0ba86e4081b4b63a57d3da617c77e5eb00127f355f121c8b24609a119ddc73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:21-ea-9-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:cfa6e6841bf783ae47523dc5cdcf17404febd9086c90bc95d4625ee7a24950bd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.0 MB (264021601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81731e6e2ce2235670641a8c226aa05903b1c1c122c61bc09af6bd8f2132948b`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 27 Jan 2023 22:41:24 GMT
ADD file:1081f67c6d4b6b053a45161b9968a0371ed81fc45f61729a33bffa9a470ec646 in / 
# Fri, 27 Jan 2023 22:41:25 GMT
CMD ["/bin/bash"]
# Fri, 27 Jan 2023 22:59:27 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 27 Jan 2023 22:59:27 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 27 Jan 2023 22:59:27 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 22:59:27 GMT
ENV LANG=en_US.UTF-8
# Fri, 10 Feb 2023 01:56:48 GMT
ENV JAVA_VERSION=21-ea+9
# Fri, 10 Feb 2023 01:57:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='50ce8bd2e9b710726e7117ba3a302287a0be51cb187721a422ee63cadbf717a2'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='86f137227e32994689e70b0a2f426adb45a16807bc84398926e841452cfe83d0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Feb 2023 01:57:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:114f8bb3e448153115527e27f088f4ed8912d567d8785d54c82dbf490230f6d0`  
		Last Modified: Fri, 27 Jan 2023 22:43:00 GMT  
		Size: 51.0 MB (51033896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc016fcb2fb8b8e69042ed80b5f1629423ef745bcb1ac72c0501de8b7b02850`  
		Last Modified: Fri, 27 Jan 2023 23:05:00 GMT  
		Size: 15.3 MB (15268160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749295ead74c534a5157f9457060231c1972503767907d31c63253d902271de4`  
		Last Modified: Fri, 10 Feb 2023 02:03:39 GMT  
		Size: 197.7 MB (197719545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
