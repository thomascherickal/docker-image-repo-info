## `openjdk:18-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:f4d58cbcaf21ada295b1aa4b094e0e36f1d89835c903fae1a5d7d1b3a308e803
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:d122b0601810133c015d9ef79df31d5840a4acd3f72dc4b3ced85659beff0c76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.5 MB (251493343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e47699f27caf73ae69bf89f340f8763362ed41684da1687d41cbc71633a8077`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 13 Oct 2021 18:30:19 GMT
ADD file:a6def617e1c0cf7def2d3ce3c79073621ed8efb37deed65fb49e7fc0a6d8ea37 in / 
# Wed, 13 Oct 2021 18:30:20 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 18:48:31 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 13 Oct 2021 18:48:31 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 13 Oct 2021 18:48:32 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 18:48:32 GMT
ENV LANG=en_US.UTF-8
# Wed, 13 Oct 2021 18:48:32 GMT
ENV JAVA_VERSION=18-ea+18
# Wed, 13 Oct 2021 18:48:43 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/18/GPL/openjdk-18-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='425b4f9afe439b4690593e5f78e27b6687525114a66f652c285a7dcca95b1961'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/18/GPL/openjdk-18-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='af5b0d66cf7c4f7450066fd67dbb0d48c17bcc5ab8ddb105cf7fe66176427f87'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 13 Oct 2021 18:48:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e0ada0403966475cc22d4e65b5fd1bde8aac848d542317ef0154b8961c767d23`  
		Last Modified: Wed, 13 Oct 2021 18:31:57 GMT  
		Size: 48.2 MB (48235779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ebd61f33542411694b578674a48c8a09f401b78b67f813518bff7eb70dbbb`  
		Last Modified: Wed, 13 Oct 2021 18:57:37 GMT  
		Size: 15.4 MB (15397943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a926785f169f325a36db72e6e40880fc82d6cf38e35260164b48750b96701e`  
		Last Modified: Wed, 13 Oct 2021 18:57:49 GMT  
		Size: 187.9 MB (187859621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:511c7d52270aabd8c2de725a2d14faa73b0bb71a4489951fac3a0e1bdff285e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (252047695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02ce3a5376ce56d509713ce6e24a3f2f77e8e876e8ae69a168f253c298123cff`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 29 Sep 2021 09:28:50 GMT
ADD file:affde62a0aaf80f490cc93e1f691166a15a32c6ef6bc21af35a6659d24c8b6ef in / 
# Wed, 29 Sep 2021 09:28:51 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 05:59:43 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 13 Oct 2021 05:59:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 13 Oct 2021 05:59:44 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 05:59:45 GMT
ENV LANG=en_US.UTF-8
# Wed, 13 Oct 2021 05:59:46 GMT
ENV JAVA_VERSION=18-ea+18
# Wed, 13 Oct 2021 06:00:08 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/18/GPL/openjdk-18-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='425b4f9afe439b4690593e5f78e27b6687525114a66f652c285a7dcca95b1961'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/18/GPL/openjdk-18-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='af5b0d66cf7c4f7450066fd67dbb0d48c17bcc5ab8ddb105cf7fe66176427f87'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 13 Oct 2021 06:00:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2f5eee715870559160403451bcd7b891478e0df052b7f9456144f3e89e5b994f`  
		Last Modified: Wed, 29 Sep 2021 09:30:28 GMT  
		Size: 48.8 MB (48828923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d586374e21f8d72195ddee3ded7c701588c9aaf00feb9feeaf6a586f435121df`  
		Last Modified: Wed, 13 Oct 2021 06:24:14 GMT  
		Size: 16.4 MB (16438619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65f58efb12589be092310702f8cbcef49bfb4bbfa3c1ebc1c7510fa77f1b8fa`  
		Last Modified: Wed, 13 Oct 2021 06:24:28 GMT  
		Size: 186.8 MB (186780153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
