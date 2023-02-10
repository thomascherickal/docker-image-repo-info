## `openjdk:20-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:b44199128081d5a4c8afed489a07781b8c93ed4c2a8a4ffec9cf909c42277288
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:8e8a9e3288895cc114f930998944a991a587100f27fec5fb037540551cce5d2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262839823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0160c66ca6d993d7503b77db37874e771f0eaf38577cdaf0d929ca519321db4b`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Fri, 27 Jan 2023 23:54:48 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 27 Jan 2023 23:55:34 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Fri, 27 Jan 2023 23:55:34 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 23:55:34 GMT
ENV LANG=en_US.UTF-8
# Thu, 02 Feb 2023 23:33:34 GMT
ENV JAVA_VERSION=20-ea+34
# Thu, 02 Feb 2023 23:33:43 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='1c8e4809d7444903dfde02ef45821c1206a5d98c241c04280434ef9b5aca15ad'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e43b2f39d2b6359755a6cd26c01057b1b6d53c84d944fc3396500b2f21a15be'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 02 Feb 2023 23:33:44 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e048d0a387420acfdb05a1ec44ed79aa01be81adcd731b3100359277ca89d08b`  
		Last Modified: Fri, 27 Jan 2023 23:38:26 GMT  
		Size: 50.5 MB (50466577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde4d617b6d23e9a10ad76ad56ca1591c532861de431f66e6e735233eef43807`  
		Last Modified: Sat, 28 Jan 2023 00:00:16 GMT  
		Size: 14.2 MB (14244027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256ecf514fe61b7881a71274f7dc15a89106fdef4ad17572b5e06cf3faa897cb`  
		Last Modified: Thu, 02 Feb 2023 23:42:28 GMT  
		Size: 198.1 MB (198129219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:db962447c6aae534acdc7734fdae63a44c5917a062af72d536d07e7a1bc17fe9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.9 MB (262932834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:431fcb51ae58662e085e8eaf67216289bdc5a47586ac893dbb2a9c390d07db30`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 27 Jan 2023 22:41:24 GMT
ADD file:1081f67c6d4b6b053a45161b9968a0371ed81fc45f61729a33bffa9a470ec646 in / 
# Fri, 27 Jan 2023 22:41:25 GMT
CMD ["/bin/bash"]
# Fri, 27 Jan 2023 22:59:27 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 27 Jan 2023 23:00:22 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Fri, 27 Jan 2023 23:00:22 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2023 23:00:22 GMT
ENV LANG=en_US.UTF-8
# Fri, 10 Feb 2023 01:58:21 GMT
ENV JAVA_VERSION=20-ea+35
# Fri, 10 Feb 2023 01:58:33 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/35/GPL/openjdk-20-ea+35_linux-x64_bin.tar.gz'; 			downloadSha256='2062453caf72cff8ad296b84d90108f2eb057d7415a5c7d109672fd6b613ef1f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/35/GPL/openjdk-20-ea+35_linux-aarch64_bin.tar.gz'; 			downloadSha256='65541ed26e56fe91b7d3ba703bde269e5568313e3e7168d2476455f03f460eda'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Feb 2023 01:58:35 GMT
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
	-	`sha256:8c7c05adc5ab3338dcbac336dd1b5bf8b758003edca27d0f9d5ef17e0fb8e09a`  
		Last Modified: Fri, 10 Feb 2023 02:07:10 GMT  
		Size: 196.6 MB (196630778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
