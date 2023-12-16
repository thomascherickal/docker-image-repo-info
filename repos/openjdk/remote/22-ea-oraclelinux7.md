## `openjdk:22-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:3d1ea74f383f1d201df55c0003e672b630c593148b9eaaf5803e096b4f3ef442
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `openjdk:22-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:2ad8aa1965efdfe5385ad3cb70cde5bb955a726eb30ca1382e42865dd008a100
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.5 MB (267458237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6efe3b669617632be6c3ce73eb69e732864eb41d346ad7ac49811a458413406`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 08 Dec 2023 19:48:25 GMT
ADD file:74b33794f8e61e810f09c38da020f9becc9f6987d22fa6f42af6b4226505e6ca in / 
# Fri, 08 Dec 2023 19:48:25 GMT
CMD ["/bin/bash"]
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 08 Dec 2023 19:48:25 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Dec 2023 19:48:25 GMT
ENV LANG=en_US.UTF-8
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:20e4dcae4c693910efbf28a556e2fa88ef717e15364f63da7e0a4a130b9b714e`  
		Last Modified: Thu, 14 Dec 2023 23:23:14 GMT  
		Size: 50.5 MB (50499235 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ae482577de06376fc16cc897d430c127d2648b8d7a3f8ee6e10fef0f89d09be9`  
		Last Modified: Fri, 15 Dec 2023 22:05:54 GMT  
		Size: 14.2 MB (14232220 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba7225dfcac291f0acbe8dd81e4d56e50284b60693316b668b738354ebca7ee4`  
		Last Modified: Fri, 15 Dec 2023 22:05:58 GMT  
		Size: 202.7 MB (202726782 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:22-ea-oraclelinux7` - unknown; unknown

```console
$ docker pull openjdk@sha256:b4e96ec30bcc6d2838ad73fcad49ebe6597686bfa12046c18dc2d42b57f3c1aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3785093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12804c2892dbfb0da92e676a816be5fbd0823c2bb1122f8580bcebc81dce4c5`

```dockerfile
```

-	Layers:
	-	`sha256:2df8ad7875e5e6a41b47b01b41dc3d2b7a42f67f9651adcfb96da0642880b8ca`  
		Last Modified: Fri, 15 Dec 2023 22:05:53 GMT  
		Size: 3.8 MB (3768690 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:86fc34fce69265dcdcbf7f7f85a0bca0e6ea71c41885dd9fb0ae2755697872e5`  
		Last Modified: Fri, 15 Dec 2023 22:05:53 GMT  
		Size: 16.4 KB (16403 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:22-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:52927d45bcadc2df49e69bf5f17f737a8eabdfaddf19c5424a8aa49f0cdb41d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.1 MB (267136889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:975b105f1bc2d9b9133ed3f11b99d95dc4200ac33dab5b5d6d38526f4f9c623d`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 08 Dec 2023 19:48:25 GMT
ADD file:7f9b20722f4f2c781b7814e113711ee10ee458be84fe343e7d61658ede9c4711 in / 
# Fri, 08 Dec 2023 19:48:25 GMT
CMD ["/bin/bash"]
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 08 Dec 2023 19:48:25 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Dec 2023 19:48:25 GMT
ENV LANG=en_US.UTF-8
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:01eab324a7fc4cacc34c78d38ce9548750df098b20899d269b500307b6765a1d`  
		Last Modified: Fri, 15 Dec 2023 00:04:16 GMT  
		Size: 51.1 MB (51110815 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f96633a794a03133d53bf43854186ba59a38c777f78fe1e7226aff149ef8d228`  
		Last Modified: Fri, 15 Dec 2023 23:21:22 GMT  
		Size: 15.2 MB (15241860 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:310ba94f0a182fa2ac30a572d5515ef81c9626f7483cd61f56849319ba2c505f`  
		Last Modified: Fri, 15 Dec 2023 23:28:07 GMT  
		Size: 200.8 MB (200784214 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:22-ea-oraclelinux7` - unknown; unknown

```console
$ docker pull openjdk@sha256:92dae1513d9f694b5375cd8eba88672a599840d0002438ff226e54e02ddf9b51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3780806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1ef7a762b8776118588658a0468df28b864460ce7b4ce491305d6d83cfd411`

```dockerfile
```

-	Layers:
	-	`sha256:9bfdd18a708067a57ad3d34360dd8c54beefa8f3e7c4c507ceb5b9e34dd9ed7e`  
		Last Modified: Fri, 15 Dec 2023 23:28:03 GMT  
		Size: 3.8 MB (3764557 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:367d692a826761ef85a97f1f797db1c770a355dc413e890318941890967ad2a5`  
		Last Modified: Fri, 15 Dec 2023 23:28:02 GMT  
		Size: 16.2 KB (16249 bytes)  
		MIME: application/vnd.in-toto+json
