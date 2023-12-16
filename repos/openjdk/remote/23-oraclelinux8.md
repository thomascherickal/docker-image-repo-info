## `openjdk:23-oraclelinux8`

```console
$ docker pull openjdk@sha256:dddd8601be1567c8d4be2d5dbfd266d7f58cee9a48dbba70942b3df4e508fc77
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `openjdk:23-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:4c88db8580f1e3540bc14e9a44cb81d89f56bbd54df832ffe81cefb7c622578b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.1 MB (269118344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55a52074de1ad4eebdeab07fa0667e1e07f99bb3e285a8553dd0ac4bf094a614`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 06 Dec 2023 19:23:17 GMT
ADD file:0fefdd26d1656281881908973318cde9ebc07674dc1098bbf40d9ce6acf2f036 in / 
# Wed, 06 Dec 2023 19:23:18 GMT
CMD ["/bin/bash"]
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-23
# Sat, 09 Dec 2023 18:45:21 GMT
ENV PATH=/usr/java/openjdk-23/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2023 18:45:21 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_VERSION=23-ea+1
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='740a84253d35402b9213bf187ee4f058817c614f8cc47cb3414e02760f05099f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='74fe7c8e67c5b80f868ec20daecb112fc090fb91c58bf4ce5297cf77c9935fa5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e9f2695d7e5b00c4289ec17d08776fb4b6664a9c805294c7d5c364b56d3b9435`  
		Last Modified: Wed, 06 Dec 2023 19:24:28 GMT  
		Size: 51.3 MB (51319965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:91b33e5f534a5b32542748b1dea922388d8461e68ea449e56b177ae2d5a6a23e`  
		Last Modified: Fri, 15 Dec 2023 22:05:47 GMT  
		Size: 15.0 MB (15003844 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b73eb92ec9e7a98113f5faddd846ccd0121d380b1bb94ad0d7bce072b80a49dc`  
		Last Modified: Fri, 15 Dec 2023 22:05:50 GMT  
		Size: 202.8 MB (202794535 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:23-oraclelinux8` - unknown; unknown

```console
$ docker pull openjdk@sha256:453470aca51189c12b26e445fe709d535a485067b7beb7486cedb2e8115608bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1935674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbd055592fa7b3777c9e7439f6f281080ea1d99545d82b3d0a00452747189b24`

```dockerfile
```

-	Layers:
	-	`sha256:e84ce719a02a7aea7c76704ac0ee6372343d5c9209217fd65e182fee88817e64`  
		Last Modified: Fri, 15 Dec 2023 22:05:47 GMT  
		Size: 1.9 MB (1915811 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:528a3e24d714b3ffce050bfff8c5e4f6357db0a16ded7b27cfbc0189a91eeacb`  
		Last Modified: Fri, 15 Dec 2023 22:05:47 GMT  
		Size: 19.9 KB (19863 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:23-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b4c47fdc5a908034b36ec92a951a7c65a214f101e30f799c6ae93e05f3b857c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.6 MB (266610052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b47ce58b3fa68aea9b5dda28a2da58c3eda51a1e738162b81adda0425748fe5b`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-23
# Sat, 09 Dec 2023 18:45:21 GMT
ENV PATH=/usr/java/openjdk-23/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2023 18:45:21 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_VERSION=23-ea+1
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='740a84253d35402b9213bf187ee4f058817c614f8cc47cb3414e02760f05099f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='74fe7c8e67c5b80f868ec20daecb112fc090fb91c58bf4ce5297cf77c9935fa5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61733c769b5e0a95819f0df3a4ff8980287c816c785b828bfb4321091a36b7f5`  
		Last Modified: Fri, 15 Dec 2023 23:19:58 GMT  
		Size: 15.7 MB (15686550 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a06248b207c18e486d099c06674570990f42bf7aea66462eef05dfcef438e231`  
		Last Modified: Fri, 15 Dec 2023 23:20:03 GMT  
		Size: 200.9 MB (200850957 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:23-oraclelinux8` - unknown; unknown

```console
$ docker pull openjdk@sha256:5f4c06652b282cf924d25e6a7c1d37f865b9c4f2399e6c1616e7f82d3399bf9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1934127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd42ac1cdd0995647763a3284b453c97ae56337c932a35906cca86eace56dae0`

```dockerfile
```

-	Layers:
	-	`sha256:d1e6636493f8bd8774366b62e7711670e92a13abb64949281416dcc60516734c`  
		Last Modified: Fri, 15 Dec 2023 23:19:58 GMT  
		Size: 1.9 MB (1914393 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6eed5529c80dba450ade49d42e2b99734c951908276b92fc18609495447ed2b2`  
		Last Modified: Fri, 15 Dec 2023 23:19:58 GMT  
		Size: 19.7 KB (19734 bytes)  
		MIME: application/vnd.in-toto+json
