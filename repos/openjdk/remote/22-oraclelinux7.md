## `openjdk:22-oraclelinux7`

```console
$ docker pull openjdk@sha256:6a6adf86864fa7b8afe4e12d3487274d497c21393c956a86099c71b10435d6b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:36cdf4b59f3ff70b8268f7ff4d2093254468a7abaf34982c7048b032ee08023b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.3 MB (270264809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfb210b1ab704bc2fd0303324714caf768c00c95431de5700db8b8a229346883`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 12 Oct 2023 21:29:07 GMT
ADD file:2726e2d5d9aaf4024ea489d9049884aa06c0c95d6111037ba29987ba029ddc44 in / 
# Thu, 12 Oct 2023 21:29:07 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 22:19:41 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 12 Oct 2023 22:19:41 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Thu, 12 Oct 2023 22:19:41 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 22:19:41 GMT
ENV LANG=en_US.UTF-8
# Sat, 28 Oct 2023 00:37:14 GMT
ENV JAVA_VERSION=22-ea+21
# Sat, 28 Oct 2023 00:37:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='cefe6f9697801dd2a7abebdbd5b7bd36ad489794589e838562da46bde434ae5e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='b77e7f170973c91690aa64a028f2e991828fde5092eabc29b602e26824216797'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 28 Oct 2023 00:37:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9ad776bc39341b015fa96ec38b0ef30213514fedd245d657d3188d81b46d367c`  
		Last Modified: Thu, 12 Oct 2023 21:30:53 GMT  
		Size: 50.5 MB (50496653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d12b7af3f237d48ffcd0cb3d2738d9661d2029fe2ac6fb20e11ead3a56ce551`  
		Last Modified: Thu, 12 Oct 2023 22:21:35 GMT  
		Size: 14.3 MB (14251137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e51d8cc617f6612524361ec14e3418f70f058940d152c63d657544d818b234e`  
		Last Modified: Sat, 28 Oct 2023 00:40:03 GMT  
		Size: 205.5 MB (205517019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f21dae34ff820c659a4cb6fa2640b449425d1cef59d2df6243feed68d6a34d2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.1 MB (270080103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6864eb2ebcebbebd7232ac86e1aeedfa062348a7f0ebb58849a68da7c70d5eca`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 12 Oct 2023 11:00:59 GMT
ADD file:67e4d2ca8c1a10f2e3e0b8cbfac921504e96756141f9a105cd73ccf06d7f1a70 in / 
# Thu, 12 Oct 2023 11:01:00 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 15:36:18 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 12 Oct 2023 15:36:18 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Thu, 12 Oct 2023 15:36:18 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 15:36:18 GMT
ENV LANG=en_US.UTF-8
# Sat, 28 Oct 2023 00:37:09 GMT
ENV JAVA_VERSION=22-ea+21
# Sat, 28 Oct 2023 00:37:22 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='cefe6f9697801dd2a7abebdbd5b7bd36ad489794589e838562da46bde434ae5e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='b77e7f170973c91690aa64a028f2e991828fde5092eabc29b602e26824216797'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 28 Oct 2023 00:37:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:71a92edb27cabcf1cd98fcea78da305dc7a1e70eb00b95534f57518084cf9823`  
		Last Modified: Thu, 12 Oct 2023 11:02:30 GMT  
		Size: 51.1 MB (51108085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd1aca6ce046cb2bd184372ec5ea080c5717e57b0cca639c9419105820a0922`  
		Last Modified: Thu, 12 Oct 2023 15:38:01 GMT  
		Size: 15.2 MB (15245141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214c9b4bddfae295a977faa9690ab3cbde236e0e7d9f02ab903d33fec952366b`  
		Last Modified: Sat, 28 Oct 2023 00:39:58 GMT  
		Size: 203.7 MB (203726877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
