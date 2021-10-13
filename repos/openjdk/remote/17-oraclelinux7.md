## `openjdk:17-oraclelinux7`

```console
$ docker pull openjdk@sha256:f36da934b224fcf1df8e3792ac74ba60d6bc3f5698b79709fceae43db643a7ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:e60a2a60659694c0e0c528888a10e31392a84b23c02649c2af2f56eb08fe9363
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.8 MB (250819470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1c544140e17d5b8cd3979e082e785c6a5b75717a0cc50e4bd3fc4e840b8f401`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 29 Sep 2021 16:28:42 GMT
ADD file:a9e7957ff3541c254a266620f438cb7ec181b31d50f939d0e687716cefdc7cf8 in / 
# Wed, 29 Sep 2021 16:28:43 GMT
CMD ["/bin/bash"]
# Wed, 29 Sep 2021 16:54:15 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 29 Sep 2021 16:55:13 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 29 Sep 2021 16:55:13 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 16:55:13 GMT
ENV LANG=en_US.UTF-8
# Wed, 29 Sep 2021 16:55:13 GMT
ENV JAVA_VERSION=17
# Wed, 29 Sep 2021 16:55:24 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-x64_bin.tar.gz'; 			downloadSha256='aef49cc7aa606de2044302e757fa94c8e144818e93487081c4fd319ca858134b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-aarch64_bin.tar.gz'; 			downloadSha256='b8108a6b6c2579bd585281937cf09d401a5a971c59b9624e18abcf596b9caa22'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 29 Sep 2021 16:55:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2294629c97e56d38612a31e50aa9a544bb9ea9a60646d016dcde035fd309dfe8`  
		Last Modified: Wed, 29 Sep 2021 16:30:26 GMT  
		Size: 48.2 MB (48241319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa27d00ff441932dc4be9fc9662577510adff660e4486fa443768e0ca6d260e`  
		Last Modified: Wed, 29 Sep 2021 17:03:16 GMT  
		Size: 15.4 MB (15433173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352238cd36927be97cb19fe1f3a8fe59466dfd575d0610ae2b7560d1c4156fb6`  
		Last Modified: Wed, 29 Sep 2021 17:05:03 GMT  
		Size: 187.1 MB (187144978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:9b5e9de49e6f94be2474c2a0ceb8dbd92146aa7c89dc72d9fa855b1f9b9d1195
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.2 MB (251219996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e15feca2006a772ffed787dafcea7cafba06d0ebfcacd38980d6fd36cb5cf2`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 29 Sep 2021 09:28:50 GMT
ADD file:affde62a0aaf80f490cc93e1f691166a15a32c6ef6bc21af35a6659d24c8b6ef in / 
# Wed, 29 Sep 2021 09:28:51 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 05:59:43 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 13 Oct 2021 06:02:52 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 13 Oct 2021 06:02:52 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 06:02:53 GMT
ENV LANG=en_US.UTF-8
# Wed, 13 Oct 2021 06:02:54 GMT
ENV JAVA_VERSION=17
# Wed, 13 Oct 2021 06:03:18 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-x64_bin.tar.gz'; 			downloadSha256='aef49cc7aa606de2044302e757fa94c8e144818e93487081c4fd319ca858134b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-aarch64_bin.tar.gz'; 			downloadSha256='b8108a6b6c2579bd585281937cf09d401a5a971c59b9624e18abcf596b9caa22'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 13 Oct 2021 06:03:18 GMT
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
	-	`sha256:b86af4fa68a5a3e6ddc5241588a0f0e4dd6338c6852c2441f52dc271fa8ef0fe`  
		Last Modified: Wed, 13 Oct 2021 06:28:53 GMT  
		Size: 186.0 MB (185952454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
