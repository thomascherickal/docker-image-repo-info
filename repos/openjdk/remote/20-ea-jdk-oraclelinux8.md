## `openjdk:20-ea-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:14eae0b50ab34818431f988dae2ce22d55e038c16bc6fb15f6af0a9cb39bf9d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:1a9409a7f753b1c36c1303bf396f582966423456512e7b38764922ddc7abede2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (249958254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201fb337745338ee4afdffed1c2400711cb4a7c47668f34ef822612b961f19e3`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:35:27 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:35:27 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 04 Aug 2022 01:35:27 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 01:35:27 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 22:51:01 GMT
ENV JAVA_VERSION=20-ea+9
# Mon, 08 Aug 2022 22:51:28 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='0d07c62c8d17ef034b26568ed71d3025cf9dcbc6b4294987e53d54cab10f549f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='13fc41a17f015ca801975625021a320b5112883194fc5dde964529894907fd83'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 22:51:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d72ac1fb23a36f89addf60367990f28d5c0882e4b8f569c77b51c51eb271261`  
		Last Modified: Thu, 04 Aug 2022 01:42:41 GMT  
		Size: 13.5 MB (13506500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42cf7a320801f642ab774ae90a06dd631bbdaff1a1d624c4bc5698bda715459a`  
		Last Modified: Mon, 08 Aug 2022 23:00:16 GMT  
		Size: 197.2 MB (197227802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f45b3e8a7b391cd5019777539ad14f56cb0007656e2c2920a9434219b9b39efa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.2 MB (248224453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7002618414e88d3c639308366042ab127ff361e2a7b05a8490cc5367c878bd`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:01:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:01:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 04 Aug 2022 01:01:13 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 01:01:14 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 23:29:46 GMT
ENV JAVA_VERSION=20-ea+9
# Mon, 08 Aug 2022 23:29:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='0d07c62c8d17ef034b26568ed71d3025cf9dcbc6b4294987e53d54cab10f549f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='13fc41a17f015ca801975625021a320b5112883194fc5dde964529894907fd83'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 23:29:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e225b6ab834ff85ee0d347a2859ecb14fc169f362360408133589ab8a37d8333`  
		Last Modified: Thu, 04 Aug 2022 01:14:59 GMT  
		Size: 14.3 MB (14278746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44516f349abc34c211463e2b6a990c2b2f5cfc954046603018baaa29061031a9`  
		Last Modified: Mon, 08 Aug 2022 23:45:45 GMT  
		Size: 195.9 MB (195922661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
