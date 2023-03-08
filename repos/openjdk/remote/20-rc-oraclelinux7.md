## `openjdk:20-rc-oraclelinux7`

```console
$ docker pull openjdk@sha256:f8305963bb2fd40211aac6fb51e0c3d4b4c59198cde08e9560d2792de2a07bc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-rc-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:8dc8baca24fea69a1c589f53a0be0cc6f246c8a4ed4baf2c1dec6964a53961a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262832928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9afcd3614227f398410e27c3ca81678d5bf416710c4897dacd699292fedd7230`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:54 GMT
ADD file:e205deb729daf99a168c27d3f97cd2b69e736fc9d4bee9ea220ec86921574a0f in / 
# Wed, 08 Mar 2023 20:22:55 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:54:26 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 08 Mar 2023 20:55:08 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 08 Mar 2023 20:55:08 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 20:55:08 GMT
ENV LANG=en_US.UTF-8
# Wed, 08 Mar 2023 20:55:08 GMT
ENV JAVA_VERSION=20
# Wed, 08 Mar 2023 20:55:17 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-x64_bin.tar.gz'; 			downloadSha256='bb863b2d542976d1ae4b7b81af3e78b1e4247a64644350b552d298d8dc5980dc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-aarch64_bin.tar.gz'; 			downloadSha256='b671dd1513e7bd4f3de6b1424a90a4998997a67593bf259936d55f5e83e31959'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 08 Mar 2023 20:55:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7b659169cb9226d08443358aa4e8147f3144614ac33f7a41217b0cf62a4d3326`  
		Last Modified: Wed, 08 Mar 2023 20:24:41 GMT  
		Size: 50.5 MB (50467964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efc12c70e0ba49ea5eb742d598c3d36a33b4d7407f8be1a8ac8641ad14e0a56`  
		Last Modified: Wed, 08 Mar 2023 20:57:27 GMT  
		Size: 14.2 MB (14236997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df66929f9a09b53011a6c76d0b672c2b82a9e0242514f534ea6d346caa5b1e0d`  
		Last Modified: Wed, 08 Mar 2023 20:58:57 GMT  
		Size: 198.1 MB (198127967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-rc-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:6898d2a18f22cb3d1f4ebe387a1e04d63857c64d9f48d74cbe68fe5ace50161d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.9 MB (262905260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b2cb881020bb7e6a8873352dc49ea58368dc23cf85a8bc649f161f7d99a0650`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:36 GMT
ADD file:d11a3555d107d9db5ab5621675aa2ecf27ec872cc591769bdc75129ff602dfd7 in / 
# Wed, 08 Mar 2023 21:02:37 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:20:32 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 08 Mar 2023 21:21:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 08 Mar 2023 21:21:12 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 21:21:12 GMT
ENV LANG=en_US.UTF-8
# Wed, 08 Mar 2023 21:21:12 GMT
ENV JAVA_VERSION=20
# Wed, 08 Mar 2023 21:21:24 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-x64_bin.tar.gz'; 			downloadSha256='bb863b2d542976d1ae4b7b81af3e78b1e4247a64644350b552d298d8dc5980dc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-aarch64_bin.tar.gz'; 			downloadSha256='b671dd1513e7bd4f3de6b1424a90a4998997a67593bf259936d55f5e83e31959'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 08 Mar 2023 21:21:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4b689a883b146569199f6bfaadce974725d68f1cd14d01950efe476637febe12`  
		Last Modified: Wed, 08 Mar 2023 21:04:11 GMT  
		Size: 51.0 MB (51027010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ce6fa2927eee2bba1cdfc5060760f859a7073e02bf271b9b61999943c2211d`  
		Last Modified: Wed, 08 Mar 2023 21:23:34 GMT  
		Size: 15.2 MB (15249325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5834a5dcd451045e5b1f318738832061ac134d8a67233550a0ff4e845124fece`  
		Last Modified: Wed, 08 Mar 2023 21:24:59 GMT  
		Size: 196.6 MB (196628925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
