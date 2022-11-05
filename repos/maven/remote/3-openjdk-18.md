## `maven:3-openjdk-18`

```console
$ docker pull maven@sha256:7204d6141a471c8a09e085643dc85d5f6f96ed63c94dd96b577e10090f19e601
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-18` - linux; amd64

```console
$ docker pull maven@sha256:2aee98b290b6fa8228054cb98b12a919ac3b7fa125c314804c90836ce07c7e28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **445.4 MB (445442104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b34b5ddbf241289a74e5a5b34e754a2bd77a6e32ea4be244695dbc875a80c0`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:07 GMT
ADD file:00e6899b8d3eccf7f795d17f9316af6ae0f3955ef2204b61bd064f5173c18357 in / 
# Fri, 04 Nov 2022 23:33:07 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:19:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 05 Nov 2022 02:20:46 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Sat, 05 Nov 2022 02:20:46 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 02:20:46 GMT
ENV LANG=C.UTF-8
# Sat, 05 Nov 2022 02:20:47 GMT
ENV JAVA_VERSION=18.0.2.1
# Sat, 05 Nov 2022 02:20:57 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 05 Nov 2022 02:20:58 GMT
CMD ["jshell"]
# Sat, 05 Nov 2022 02:59:35 GMT
RUN microdnf install findutils git
# Sat, 05 Nov 2022 02:59:36 GMT
ARG MAVEN_VERSION=3.8.6
# Sat, 05 Nov 2022 02:59:36 GMT
ARG USER_HOME_DIR=/root
# Sat, 05 Nov 2022 02:59:36 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Sat, 05 Nov 2022 02:59:36 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Sat, 05 Nov 2022 02:59:44 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 05 Nov 2022 02:59:44 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 05 Nov 2022 02:59:44 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 05 Nov 2022 02:59:45 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 05 Nov 2022 02:59:45 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 05 Nov 2022 02:59:45 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 05 Nov 2022 02:59:45 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:feec22b5b79860f47a87861bed3a29d5431a279cc239b44a2522a9ab5459d844`  
		Last Modified: Fri, 04 Nov 2022 23:34:48 GMT  
		Size: 40.6 MB (40580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab968c9bcaf076780e21bb249a61cd5dfda4716508c17678f3082057a3c9b8f8`  
		Last Modified: Sat, 05 Nov 2022 02:23:30 GMT  
		Size: 12.2 MB (12229784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9c81bf0e32371a27f88a0c073e7ad8e547174b91403d9cb61f3fe3a3fe682d`  
		Last Modified: Sat, 05 Nov 2022 02:25:17 GMT  
		Size: 188.7 MB (188744810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba63ccda1467318c08b9b96a15e2a3672dc85d11e61da3c98b8c0b25e6580e7`  
		Last Modified: Sat, 05 Nov 2022 03:02:11 GMT  
		Size: 195.1 MB (195145872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c58a440396d3307acead334307a1eb3c4640a0460282e151210a0675bff147e`  
		Last Modified: Sat, 05 Nov 2022 03:01:57 GMT  
		Size: 8.7 MB (8739506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2dfcf435144bee36eca0285ae4b68818ad6041172e02ea11a8fe5a5ea40327`  
		Last Modified: Sat, 05 Nov 2022 03:01:56 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b11a1d74e2d20d12b69257466adf4a57eaecfeddec88d03cee52e7851eb0160`  
		Last Modified: Sat, 05 Nov 2022 03:01:56 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-18` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:4ffd139c21aba80c63e95ce8b0d02b6ee4ee49e01890d36adf27b37e38c7d279
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.2 MB (455249800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b37d00e6fcb72a28f0c2932d83326394a4fb95a9e5ef446961cf24abf0bbd72`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 04 Nov 2022 22:50:08 GMT
ADD file:efa6454225ba5be177493364c69d425968d42231b708b5d492a41f9ab14d64f4 in / 
# Fri, 04 Nov 2022 22:50:08 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 00:48:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 05 Nov 2022 00:50:48 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Sat, 05 Nov 2022 00:50:48 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 00:50:48 GMT
ENV LANG=C.UTF-8
# Sat, 05 Nov 2022 00:50:48 GMT
ENV JAVA_VERSION=18.0.2.1
# Sat, 05 Nov 2022 00:50:57 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 05 Nov 2022 00:50:58 GMT
CMD ["jshell"]
# Sat, 05 Nov 2022 02:01:17 GMT
RUN microdnf install findutils git
# Sat, 05 Nov 2022 02:01:19 GMT
ARG MAVEN_VERSION=3.8.6
# Sat, 05 Nov 2022 02:01:19 GMT
ARG USER_HOME_DIR=/root
# Sat, 05 Nov 2022 02:01:19 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Sat, 05 Nov 2022 02:01:20 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Sat, 05 Nov 2022 02:01:25 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 05 Nov 2022 02:01:25 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 05 Nov 2022 02:01:25 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 05 Nov 2022 02:01:25 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 05 Nov 2022 02:01:26 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 05 Nov 2022 02:01:26 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 05 Nov 2022 02:01:26 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a13cd8cb50ab4c8c5cb15a9929fa5faf1b7833f87c827551a9a54e84789b1e0b`  
		Last Modified: Fri, 04 Nov 2022 22:51:35 GMT  
		Size: 39.4 MB (39401738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2b575a486b4b7df2602a19466f69783be33126ccdea7a939dbef7ecc85a7c7`  
		Last Modified: Sat, 05 Nov 2022 00:53:50 GMT  
		Size: 13.0 MB (13049666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedc660ff45bfd209b0ac28ae7621b270c6275e79147e8f130e3a6ee92f8860b`  
		Last Modified: Sat, 05 Nov 2022 00:55:29 GMT  
		Size: 187.7 MB (187659341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2707e5f6c44a48aa9dd1daf8b47c27197441b0258977170c8a0a0864d2ea1b99`  
		Last Modified: Sat, 05 Nov 2022 02:03:10 GMT  
		Size: 206.4 MB (206398343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c6573464ec3ad1638ddd93e4940e9a78b9577cef586b3bc4fc55a68fea7eb7`  
		Last Modified: Sat, 05 Nov 2022 02:02:59 GMT  
		Size: 8.7 MB (8739500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e07b27c9a3fec33549fe4775075b3b1a5cd621b2fb659f2d5ea05dc9c9e900`  
		Last Modified: Sat, 05 Nov 2022 02:02:58 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078afe35034928f0ed1b46f0febaa58ac1b6d4b1258a96a4d255a93575e8673e`  
		Last Modified: Sat, 05 Nov 2022 02:02:59 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
