## `openjdk:22-ea-oraclelinux8`

```console
$ docker pull openjdk@sha256:8a222219879e93d13b891453ee84e82eedfa17eb50af038e8f8fac7f5b13baee
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `openjdk:22-ea-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:ecd751b00d7b5a3c729ee05c6011865fafdee5ca6551358bead75791a6a3c3f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.1 MB (269050613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d7f90edde178c52d2abea6cf8de22606a22461d9c4bd992c06ebbdddd2d77ff`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 06 Dec 2023 19:23:17 GMT
ADD file:0fefdd26d1656281881908973318cde9ebc07674dc1098bbf40d9ce6acf2f036 in / 
# Wed, 06 Dec 2023 19:23:18 GMT
CMD ["/bin/bash"]
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 08 Dec 2023 19:48:25 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Dec 2023 19:48:25 GMT
ENV LANG=C.UTF-8
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e9f2695d7e5b00c4289ec17d08776fb4b6664a9c805294c7d5c364b56d3b9435`  
		Last Modified: Wed, 06 Dec 2023 19:24:28 GMT  
		Size: 51.3 MB (51319965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9b1a6a56d42fcfe1b52296ab972d121072a15141aded9a45a81ded78b172d158`  
		Last Modified: Fri, 15 Dec 2023 22:05:59 GMT  
		Size: 15.0 MB (15003874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f6050bba1ccc19242d2d8125082ac6be182bd39d977052a76d94e81dcbd15b4`  
		Last Modified: Fri, 15 Dec 2023 22:06:05 GMT  
		Size: 202.7 MB (202726774 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:22-ea-oraclelinux8` - unknown; unknown

```console
$ docker pull openjdk@sha256:d9c2894ca6d5b71daa6e8e4358670cc856655b6262e39b1c524e6015772d1ee9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1935720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ced8fb31217f42373e7d19d60fbfb536d30f68582d7e2b025fe40648b367177`

```dockerfile
```

-	Layers:
	-	`sha256:3cd2709e246bdf7af96114957557fe1f6c9e24274cec97aa2bdeb746020ea864`  
		Last Modified: Fri, 15 Dec 2023 22:05:59 GMT  
		Size: 1.9 MB (1915831 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f099feba4c7b1e98b06fb6b770255639f0ce2ef3512d7bfaebc1187d4170f6e6`  
		Last Modified: Fri, 15 Dec 2023 22:05:59 GMT  
		Size: 19.9 KB (19889 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:22-ea-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:9dc9e36ad9089d83956f9b1ddb434c7bde45df22e09317b646d6f4b06fd90c38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.5 MB (266543389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:216cad1a50d9524c2d3a70c9e6732e519a682602ec4bee08731f2cee4558c564`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 08 Dec 2023 19:48:25 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Dec 2023 19:48:25 GMT
ENV LANG=C.UTF-8
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
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
	-	`sha256:f502e782da1ddb3b75b59e5f91a41ff7b4d196c30a6510b24b3de9d3c1f48f3a`  
		Last Modified: Fri, 15 Dec 2023 23:27:19 GMT  
		Size: 200.8 MB (200784294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:22-ea-oraclelinux8` - unknown; unknown

```console
$ docker pull openjdk@sha256:52e5d8a3472dc411672b836f8d3c160f8901cb03bc4239543ec265c7e29dc3ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1934165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:946287e8c3735b745013891af07ba61ca39f8caf96977ea67d132f9626fb3974`

```dockerfile
```

-	Layers:
	-	`sha256:d27afab968e3c223d4fa063c4f1240ac72a4a3fe0c21e175d3dbc6da7097d513`  
		Last Modified: Fri, 15 Dec 2023 23:27:15 GMT  
		Size: 1.9 MB (1914405 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:88e0ef92b213d5007c2ed2246f495c1e59b315ffcb2c5a6c06516ad16cd19144`  
		Last Modified: Fri, 15 Dec 2023 23:27:14 GMT  
		Size: 19.8 KB (19760 bytes)  
		MIME: application/vnd.in-toto+json
