## `openjdk:21-ea-15-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:e54ae8923494f76655746ad9c0e44f562cacef6bd2d9ef66dd72d937c0857ac5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:21-ea-15-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:80b6cc788f96b50874b7f80d495234b2893e463bde42193c44f868089c2c7665
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266311016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97cb3e920bad16f5ceba76cc0d72adb51bfa62745b8a9ed2ec56dbdd03e8bc08`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Mar 2023 19:44:52 GMT
ADD file:a9428dda3ec7ae554537bb583832aa2d30484c863bf95c68e460df5858c4c0bf in / 
# Tue, 21 Mar 2023 19:44:53 GMT
CMD ["/bin/bash"]
# Tue, 21 Mar 2023 21:03:26 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 21 Mar 2023 21:03:26 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Tue, 21 Mar 2023 21:03:26 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Mar 2023 21:03:27 GMT
ENV LANG=en_US.UTF-8
# Mon, 27 Mar 2023 22:47:33 GMT
ENV JAVA_VERSION=21-ea+15
# Mon, 27 Mar 2023 22:47:46 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/15/GPL/openjdk-21-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='0fec1002b8c8975b181bd6966a817028d6b373cbc759254231f9b96db1fe6edd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/15/GPL/openjdk-21-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='93cc1eb6202093a127f1f9ed2e866a51dff29321f878085c18f317cefb113ffc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 27 Mar 2023 22:47:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:41dbc375a859f3e982b6147e2fd05b413e6995b4b728c27f1b851f64a31c004c`  
		Last Modified: Tue, 21 Mar 2023 19:45:30 GMT  
		Size: 51.0 MB (51027591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7ddfee215622f57465bb8dace7332092902d9c16c5bfa61ec64821d8cbb5c`  
		Last Modified: Tue, 21 Mar 2023 21:04:45 GMT  
		Size: 15.2 MB (15249122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70aceb63bb2c892c80155ec624c331102d707c733bcfc8d4bde9260f31a3984`  
		Last Modified: Mon, 27 Mar 2023 22:50:03 GMT  
		Size: 200.0 MB (200034303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
