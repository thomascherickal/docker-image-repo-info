## `openjdk:23-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:40c41227da221b5f5b111471165f022240353461c389418f7544805ceaff3bd6
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `openjdk:23-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:e009d3741f5effbc1b45eb5e071f9ce2eee37afd9547b53f96d59f6a10fb1df7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.5 MB (267525882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f994716dc4891dbb28256725cbfd06b60bdf9afe3c6a902dfa391395e44753a5`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 09 Dec 2023 18:45:21 GMT
ADD file:74b33794f8e61e810f09c38da020f9becc9f6987d22fa6f42af6b4226505e6ca in / 
# Sat, 09 Dec 2023 18:45:21 GMT
CMD ["/bin/bash"]
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-23
# Sat, 09 Dec 2023 18:45:21 GMT
ENV PATH=/usr/java/openjdk-23/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2023 18:45:21 GMT
ENV LANG=en_US.UTF-8
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_VERSION=23-ea+1
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='740a84253d35402b9213bf187ee4f058817c614f8cc47cb3414e02760f05099f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='74fe7c8e67c5b80f868ec20daecb112fc090fb91c58bf4ce5297cf77c9935fa5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:20e4dcae4c693910efbf28a556e2fa88ef717e15364f63da7e0a4a130b9b714e`  
		Last Modified: Thu, 14 Dec 2023 23:23:14 GMT  
		Size: 50.5 MB (50499235 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cdca5f99c2f4e73cd65de1bee7086b1d8b411fcfdc1f45cdc434d648a29a7337`  
		Last Modified: Fri, 15 Dec 2023 22:05:38 GMT  
		Size: 14.2 MB (14232144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5463cae8fa10201245ada856dce8ca1b011ba02a0a19a80b8f8199cd7498b73`  
		Last Modified: Fri, 15 Dec 2023 22:05:41 GMT  
		Size: 202.8 MB (202794503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:23-jdk-oraclelinux7` - unknown; unknown

```console
$ docker pull openjdk@sha256:3b4a5317aaa5c67aa162b76f717075ca1883bcc2c1adf411ad8419b6899752b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3785064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33546323d2a1aac128b1cef0d00e854a8f9e0ea14f7764c6441a06603d8bac7c`

```dockerfile
```

-	Layers:
	-	`sha256:7b4c78823d2e85e8ac9e9d124ecbc12f995dcb3f73b1abf23e5b7d0f3480a0df`  
		Last Modified: Fri, 15 Dec 2023 22:05:37 GMT  
		Size: 3.8 MB (3768678 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eb8af107d7c3abaad83d5e6a121a7fc6f7837198babd19f57c8c318077d6198e`  
		Last Modified: Fri, 15 Dec 2023 22:05:37 GMT  
		Size: 16.4 KB (16386 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:23-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7323b709abccdc105123880afb8b0a5c95027755366cceadd47970f589340167
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.2 MB (267203648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ced48acb0448a57972250078ded703e6fbe08ab88797e59d0a6511ca843d2e7`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 09 Dec 2023 18:45:21 GMT
ADD file:7f9b20722f4f2c781b7814e113711ee10ee458be84fe343e7d61658ede9c4711 in / 
# Sat, 09 Dec 2023 18:45:21 GMT
CMD ["/bin/bash"]
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-23
# Sat, 09 Dec 2023 18:45:21 GMT
ENV PATH=/usr/java/openjdk-23/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2023 18:45:21 GMT
ENV LANG=en_US.UTF-8
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_VERSION=23-ea+1
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='740a84253d35402b9213bf187ee4f058817c614f8cc47cb3414e02760f05099f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='74fe7c8e67c5b80f868ec20daecb112fc090fb91c58bf4ce5297cf77c9935fa5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:01eab324a7fc4cacc34c78d38ce9548750df098b20899d269b500307b6765a1d`  
		Last Modified: Fri, 15 Dec 2023 00:04:16 GMT  
		Size: 51.1 MB (51110815 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f96633a794a03133d53bf43854186ba59a38c777f78fe1e7226aff149ef8d228`  
		Last Modified: Fri, 15 Dec 2023 23:21:22 GMT  
		Size: 15.2 MB (15241860 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c2d884ed239eb256c543a322ee865b8abed40d62d90d4cfba9bade3795cb8de`  
		Last Modified: Fri, 15 Dec 2023 23:21:27 GMT  
		Size: 200.9 MB (200850973 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:23-jdk-oraclelinux7` - unknown; unknown

```console
$ docker pull openjdk@sha256:8ad0f8b71c3dd75c696535a6a2a3bcebe7dec7f5cfe58256cb4599c94383d3e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3780953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1446b0f3164d2d4f8fdf71b598951d8cefa3e3e4ed8282adea11357afdc69029`

```dockerfile
```

-	Layers:
	-	`sha256:55acd14c7a4b06783779305e13ecfd8d6b8d5da42ed67d8658c5df2062599f45`  
		Last Modified: Fri, 15 Dec 2023 23:21:22 GMT  
		Size: 3.8 MB (3764553 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:de1469713b6feb6a320dc742f8abf6446d530a61508cbab4a165bd4cdf694571`  
		Last Modified: Fri, 15 Dec 2023 23:21:21 GMT  
		Size: 16.4 KB (16400 bytes)  
		MIME: application/vnd.in-toto+json
