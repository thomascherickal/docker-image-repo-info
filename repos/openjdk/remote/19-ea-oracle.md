## `openjdk:19-ea-oracle`

```console
$ docker pull openjdk@sha256:fdc4d534a1fb41a56e7903f30688c41b7055dc9314989856a0a0cdd816f4553e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:162167a6cb62c6190c5627013dd07b4d3543d9484c1b907c05897e79fc431dfe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.5 MB (248469424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5650f3536bcf0d3a2f21b8a81b17b2abe9c53dec7796e4828815cda52378789`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 17 May 2022 22:41:42 GMT
ADD file:bbaf69bdffd0f506e447fbc52dca450a8966d950b8fa9aebd3a1bd5bd98f8b28 in / 
# Tue, 17 May 2022 22:41:42 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 22:58:38 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 17 May 2022 22:58:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 17 May 2022 22:58:38 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 May 2022 22:58:38 GMT
ENV LANG=C.UTF-8
# Wed, 18 May 2022 01:51:26 GMT
ENV JAVA_VERSION=19-ea+22
# Wed, 18 May 2022 01:51:37 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/22/GPL/openjdk-19-ea+22_linux-x64_bin.tar.gz'; 			downloadSha256='38430a128f794293c22ccaadbf7528f60a021055de72d33e210e9cf8e3a12aa6'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/22/GPL/openjdk-19-ea+22_linux-aarch64_bin.tar.gz'; 			downloadSha256='6884df76f084c7c190b86bac76643132226ba99ebbb61352b1050494fae20e17'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 18 May 2022 01:51:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:90a00d516db16c568d3da8e0a7a5a78fa6fef5a39f3d688f831d254b77791565`  
		Last Modified: Tue, 17 May 2022 22:42:38 GMT  
		Size: 39.2 MB (39220501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fc60984518a14e9454222efb6ec0a4e8c3d479f4aaf21961fa45df6b0622e3`  
		Last Modified: Tue, 17 May 2022 23:05:19 GMT  
		Size: 13.5 MB (13504594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d40557dff1447a5d4482d2de26747d2d7559030dfe44f15f65f3db53e08ec6`  
		Last Modified: Wed, 18 May 2022 01:57:42 GMT  
		Size: 195.7 MB (195744329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:81113950aa793d7a25eca59b023395307843460ef2cbc6ae77639cbb53bb7741
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.8 MB (246829289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02e4f5e84a47c65d6262b7e94886fa971c912e420b26715bffcbe925af82e742`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 17 May 2022 22:52:38 GMT
ADD file:263fe8ce0663428b324fa2909814084a77bf17118d772058d41546b804a4b968 in / 
# Tue, 17 May 2022 22:52:39 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 23:12:08 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 17 May 2022 23:12:08 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 17 May 2022 23:12:09 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 May 2022 23:12:10 GMT
ENV LANG=C.UTF-8
# Fri, 20 May 2022 21:03:21 GMT
ENV JAVA_VERSION=19-ea+23
# Fri, 20 May 2022 21:03:39 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/23/GPL/openjdk-19-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='37187e2eecb64237757cf5d5b2c7a94b25d2b03f3ea5b12bf77a5fe8b1508ac4'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/23/GPL/openjdk-19-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad7e6c255a6a0fcb02b05a879036c1d3029693c577b7cc97323f7e43901e48e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 20 May 2022 21:03:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0dbddf5847a3e154a061766ddebe6a3cae471c97cabb3be2871f6d91f265d137`  
		Last Modified: Tue, 17 May 2022 22:53:43 GMT  
		Size: 38.0 MB (38012703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6f1a9466bd7ec91933e510c0258839b2df2301b1d385203492a27a3d66f0ab`  
		Last Modified: Tue, 17 May 2022 23:23:18 GMT  
		Size: 14.3 MB (14273985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be4bf27d4c67027653fd3a497643a54f80affadeb71351539fdc526c94b90e2`  
		Last Modified: Fri, 20 May 2022 21:16:21 GMT  
		Size: 194.5 MB (194542601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
