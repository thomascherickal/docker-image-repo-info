## `openjdk:22-ea-jdk-oracle`

```console
$ docker pull openjdk@sha256:b6898f62a2fbbcbd7fec27732ccb8e269c7b79b804a5ec687239c4f3807a7175
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `openjdk:22-ea-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:fdf374895b517a9e396ddef76de49dbd527a328c7cea7a43a0e65da13323a9a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.0 MB (269044192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c70228bfc4828c4330cf1344c64b24b5c8847ab1ce2cd467e3cff1834b62cd0c`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 15 Dec 2023 19:48:12 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Fri, 15 Dec 2023 19:48:12 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 19:48:12 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all # buildkit
# Fri, 15 Dec 2023 19:48:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 15 Dec 2023 19:48:12 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:48:12 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 19:48:12 GMT
ENV JAVA_VERSION=22-ea+28
# Fri, 15 Dec 2023 19:48:12 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/28/GPL/openjdk-22-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='c19197168f6e8f67635539f348e7e97ebf21cacda670bec9304e59cb9e967fd1'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/28/GPL/openjdk-22-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='cfc0261560182c1fb0e8e6ab133a6300aa3da0663abdf5f195f7a664f8f7d56e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 15 Dec 2023 19:48:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bff7b8fbce30b40333aaedc0b91137c6e2e4674bbbdb5ee74bab9446498d3cda`  
		Last Modified: Thu, 21 Dec 2023 00:40:49 GMT  
		Size: 15.0 MB (14995398 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:91f34707a5f47f7d1f42ed630f919090c20ebd5707a02171e3df7f9b04fc10f4`  
		Last Modified: Thu, 21 Dec 2023 00:40:51 GMT  
		Size: 202.7 MB (202725326 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:22-ea-jdk-oracle` - unknown; unknown

```console
$ docker pull openjdk@sha256:cb09984857f640e9a2cf815c2f3431fae942cf1f52038d497c1d51d853df7c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1935740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75d5ebe9c95afa2b1684d5bdd895389e9f4c351c1c862d94e3c30ab257c9ee77`

```dockerfile
```

-	Layers:
	-	`sha256:375caee7e627e1cfa81c3d4c36268b7b75ebccb6b7d7b33a9ffd1bbe976af116`  
		Last Modified: Thu, 21 Dec 2023 00:40:48 GMT  
		Size: 1.9 MB (1915851 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:beb862590901c93e0a338c78d4563ed6a865952fe82cfd9f7217973b2dd75408`  
		Last Modified: Thu, 21 Dec 2023 00:40:47 GMT  
		Size: 19.9 KB (19889 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:22-ea-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:96fb735674b056117c4fd9d8bafa2326bd337c9e1ddee670660c026412090f38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.6 MB (266554803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca283082377aebcbfa5d05fb45d6c26aad10076968fe7f920e704634e5c35c4d`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 15 Dec 2023 19:48:12 GMT
ADD file:b736c1bb75174fcadec81f68a30d2db09432c3999d3df92c07c057a5cc8b07a6 in / 
# Fri, 15 Dec 2023 19:48:12 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 19:48:12 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all # buildkit
# Fri, 15 Dec 2023 19:48:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 15 Dec 2023 19:48:12 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:48:12 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 19:48:12 GMT
ENV JAVA_VERSION=22-ea+28
# Fri, 15 Dec 2023 19:48:12 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/28/GPL/openjdk-22-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='c19197168f6e8f67635539f348e7e97ebf21cacda670bec9304e59cb9e967fd1'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/28/GPL/openjdk-22-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='cfc0261560182c1fb0e8e6ab133a6300aa3da0663abdf5f195f7a664f8f7d56e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 15 Dec 2023 19:48:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f065eb68ef2e8ae9b60daa693d770aedc4bf77fb5bacc4b006960acc8eb01f28`  
		Last Modified: Wed, 20 Dec 2023 22:54:12 GMT  
		Size: 50.1 MB (50079714 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e51f352f0f1de3c800e109fad5b2dae0cb9097249a14ca89d420642f858cc188`  
		Last Modified: Thu, 21 Dec 2023 07:07:40 GMT  
		Size: 15.7 MB (15690041 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e45774984024564516230ff8cf70c9589e05d4ebc28e94b2c7faf68513f9e882`  
		Last Modified: Thu, 21 Dec 2023 07:08:34 GMT  
		Size: 200.8 MB (200785048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:22-ea-jdk-oracle` - unknown; unknown

```console
$ docker pull openjdk@sha256:04837698de94c203346c49d304537bfa50fe2af7978eebea519f7764de1d1ee3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1934185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a98cc400f992bcfe6ef889dd50809bdd8c556ed73b9a2e6eed593526eb6b8b6e`

```dockerfile
```

-	Layers:
	-	`sha256:9c47afabb5db1b9343dc15f978804b30a29a455bac31cd6b15e0e513a280d0e5`  
		Last Modified: Thu, 21 Dec 2023 07:08:29 GMT  
		Size: 1.9 MB (1914425 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eab2d90296dddce461efc287bb203cd6f06d3ae20c1fa1fefd87e5f3b41ec153`  
		Last Modified: Thu, 21 Dec 2023 07:08:28 GMT  
		Size: 19.8 KB (19760 bytes)  
		MIME: application/vnd.in-toto+json
