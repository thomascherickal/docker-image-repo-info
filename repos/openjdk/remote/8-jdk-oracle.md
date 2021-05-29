## `openjdk:8-jdk-oracle`

```console
$ docker pull openjdk@sha256:5baeb41771bda209dda31a4bf111b3a1504d2977f378c6dc2bb0a09a41a4917e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:8-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:d29aa153eb3df3445aa6a10607fff04bdad051b297d3f0f4205d0916804fffce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.4 MB (161412954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a199e431fee21d245a0ac315ab6fa66239db10d825b83a389a7461fae79e57f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 28 May 2021 18:22:12 GMT
ADD file:9e4bcf8e1c3b7657912e93a0b82bf37752a310fa3041ec461562c85d65529ad3 in / 
# Fri, 28 May 2021 18:22:12 GMT
CMD ["/bin/bash"]
# Fri, 28 May 2021 18:39:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 28 May 2021 18:41:06 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Fri, 28 May 2021 18:41:06 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 May 2021 18:41:06 GMT
ENV LANG=C.UTF-8
# Fri, 28 May 2021 18:41:07 GMT
ENV JAVA_VERSION=8u292
# Fri, 28 May 2021 18:41:14 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_linux_8u292b10.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:daa797b1cf01195cd47497fc9ddbf3fc4404f3fc012110f206b7fa3dd531e43d`  
		Last Modified: Fri, 28 May 2021 18:23:25 GMT  
		Size: 42.2 MB (42183040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7f736a217a7dd2e90a8ba647050e6374f7c3f746ad3256682302739a73ee7`  
		Last Modified: Fri, 28 May 2021 18:44:27 GMT  
		Size: 13.4 MB (13401079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e89adf60f965af42e619ed8a9d68b73cc121a2785f507ca657893a202124c01`  
		Last Modified: Fri, 28 May 2021 18:48:27 GMT  
		Size: 105.8 MB (105828835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:76f2accc6d01801315bbf04f4b09f7a1ab7b224bdf1bf00d3b7b9d3d1cc5c25e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.1 MB (161105554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b82f7a9c790d55066a2b3a4e4f09f17961354ccdb4e1563761a4ba70f6b2dae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 28 May 2021 18:41:46 GMT
ADD file:11d6c70bf365c2598abfb596f813afaa1a3030212b79ad6c9e239dc94fdd932a in / 
# Fri, 28 May 2021 18:41:47 GMT
CMD ["/bin/bash"]
# Fri, 28 May 2021 18:59:41 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 28 May 2021 19:04:26 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Fri, 28 May 2021 19:04:26 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 May 2021 19:04:26 GMT
ENV LANG=C.UTF-8
# Fri, 28 May 2021 19:04:26 GMT
ENV JAVA_VERSION=8u292
# Fri, 28 May 2021 19:04:33 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_linux_8u292b10.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:6bb7bddcd571a468c93282c3fa3b0e38fdcf15ee58fec20d63d32da56f3074af`  
		Last Modified: Fri, 28 May 2021 18:43:06 GMT  
		Size: 42.1 MB (42054735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1363fd6ea5b7069bbb5efb69721e5fbb5c89d4cf037ed7b6b6ed1476fa5ad8`  
		Last Modified: Fri, 28 May 2021 19:11:54 GMT  
		Size: 14.2 MB (14173117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6bf961ab63aa1e7132810e664c927103ee5b0c1e0d0ced646324490c581957`  
		Last Modified: Fri, 28 May 2021 19:19:13 GMT  
		Size: 104.9 MB (104877702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
