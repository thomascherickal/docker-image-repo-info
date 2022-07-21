## `maven:3-openjdk-18`

```console
$ docker pull maven@sha256:2bbc0012d75b730146421b428037459886e8f4f79e76e2be26d753f8e8a1ceb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-18` - linux; amd64

```console
$ docker pull maven@sha256:d70c3e9eb31ba34e612e933e69e4ae8d2ad3e1ba7b1b9e0055199f32adf761e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.8 MB (436782453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04433fce093c2d2132169c202f6d9343a164c1c5b3322715541ed82a20537b83`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:34 GMT
ADD file:69555d6633d88e50ab2ddecc8bc5002a8f79005d828a9093975d68ca05b023e9 in / 
# Tue, 05 Jul 2022 22:20:34 GMT
CMD ["/bin/bash"]
# Tue, 05 Jul 2022 22:49:44 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 05 Jul 2022 22:51:26 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Tue, 05 Jul 2022 22:51:26 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Jul 2022 22:51:26 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jul 2022 00:40:10 GMT
ENV JAVA_VERSION=18.0.2
# Thu, 21 Jul 2022 00:40:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2/f6ad4b4450fd4d298113270ec84f30ee/9/GPL/openjdk-18.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='cf06f41a3952038df0550e8cbc2baf0aa877c3ba00cca0dd26f73134f8baf0e6'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2/f6ad4b4450fd4d298113270ec84f30ee/9/GPL/openjdk-18.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='99d994dab3c5ad0e87a3d72dc3be33d5b2f045f0ddda0cb7853dfbf6b5d5d3b0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 21 Jul 2022 00:40:21 GMT
CMD ["jshell"]
# Thu, 21 Jul 2022 01:20:36 GMT
RUN microdnf install findutils git
# Thu, 21 Jul 2022 01:20:37 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 21 Jul 2022 01:20:37 GMT
ARG USER_HOME_DIR=/root
# Thu, 21 Jul 2022 01:20:38 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 21 Jul 2022 01:20:38 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 21 Jul 2022 01:20:40 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 21 Jul 2022 01:20:40 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 21 Jul 2022 01:20:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 21 Jul 2022 01:20:40 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 21 Jul 2022 01:20:40 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 21 Jul 2022 01:20:40 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 21 Jul 2022 01:20:40 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e54b73e95ef388354463a761e4e93ce3dac29cb244b2dc0424f2f4afc6ddf5cd`  
		Last Modified: Tue, 05 Jul 2022 22:21:41 GMT  
		Size: 39.2 MB (39222121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e62647f09f0ab1a3ac2d84823777bead33aa8e201c13b86c063296e8268023`  
		Last Modified: Tue, 05 Jul 2022 22:58:01 GMT  
		Size: 13.5 MB (13505357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439f00ba91854f117a61b0a30122dae26715969f49e2e0bce2566ef54717be66`  
		Last Modified: Thu, 21 Jul 2022 00:47:36 GMT  
		Size: 188.7 MB (188739940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bb35ad43a716fada8a31a0725873bcc3d1ca0b550214b340cd4ef9a20c905f`  
		Last Modified: Thu, 21 Jul 2022 01:23:24 GMT  
		Size: 186.6 MB (186574316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881f8208530a4f6e157720a371090c63da61bd2694cd58b5c29760f3963a9f49`  
		Last Modified: Thu, 21 Jul 2022 01:23:09 GMT  
		Size: 8.7 MB (8739502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d5c145c3176c734471701b2abe3a2273ecfd7c55228467b3a2fc236fe0b92a`  
		Last Modified: Thu, 21 Jul 2022 01:23:09 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f585ccfbbb3c175c2dca096735fb444f663defe378a027a06561145d6bfc8cc`  
		Last Modified: Thu, 21 Jul 2022 01:23:10 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-18` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:811fb733e499bed9109d677031615cf5ddc44269a58350d2813caed45c6b708c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **442.9 MB (442929912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c43b2998382605450c3d5558f4cf88ac21099fe95a36f8e8839a1a6c68e9172e`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:14 GMT
ADD file:e864e9187ff57bc1df9611a0990052f89611bfe7b6bc8e3d24b500b0886ec725 in / 
# Tue, 05 Jul 2022 22:43:14 GMT
CMD ["/bin/bash"]
# Tue, 05 Jul 2022 23:04:00 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 05 Jul 2022 23:07:26 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Tue, 05 Jul 2022 23:07:27 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Jul 2022 23:07:28 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jul 2022 01:15:52 GMT
ENV JAVA_VERSION=18.0.2
# Thu, 21 Jul 2022 01:16:06 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2/f6ad4b4450fd4d298113270ec84f30ee/9/GPL/openjdk-18.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='cf06f41a3952038df0550e8cbc2baf0aa877c3ba00cca0dd26f73134f8baf0e6'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2/f6ad4b4450fd4d298113270ec84f30ee/9/GPL/openjdk-18.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='99d994dab3c5ad0e87a3d72dc3be33d5b2f045f0ddda0cb7853dfbf6b5d5d3b0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 21 Jul 2022 01:16:06 GMT
CMD ["jshell"]
# Thu, 21 Jul 2022 02:28:55 GMT
RUN microdnf install findutils git
# Thu, 21 Jul 2022 02:28:56 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 21 Jul 2022 02:28:56 GMT
ARG USER_HOME_DIR=/root
# Thu, 21 Jul 2022 02:28:57 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 21 Jul 2022 02:28:58 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 21 Jul 2022 02:29:01 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 21 Jul 2022 02:29:02 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 21 Jul 2022 02:29:03 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 21 Jul 2022 02:29:05 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 21 Jul 2022 02:29:06 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 21 Jul 2022 02:29:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 21 Jul 2022 02:29:07 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e5d41499b4049578ed8bbb14817cd79d4136a84899b65e4364b0125d4d1c792c`  
		Last Modified: Tue, 05 Jul 2022 22:44:31 GMT  
		Size: 38.0 MB (38027757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622a5406eea6948259fe9d62dd3f3f40ef71254cb260355242ef51e23880970`  
		Last Modified: Tue, 05 Jul 2022 23:20:55 GMT  
		Size: 14.3 MB (14282866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7b28fa4ad8112825b080278f07c407ea876d45e9177864351b8ef0dbcab33d`  
		Last Modified: Thu, 21 Jul 2022 01:29:32 GMT  
		Size: 187.7 MB (187664261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0cb6c7e55914bd84256b7b17624841e5228efc5ce22847d8547a0866d746ba`  
		Last Modified: Thu, 21 Jul 2022 02:33:32 GMT  
		Size: 194.2 MB (194214366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4217a23ef5e335efae106a6764cffa3f49572513e2dea441f32d8964d954d6e0`  
		Last Modified: Thu, 21 Jul 2022 02:33:15 GMT  
		Size: 8.7 MB (8739445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a360041356b3129118d41364859f0bc463ecac5e3f44421c3f22923c3938f7`  
		Last Modified: Thu, 21 Jul 2022 02:33:14 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3999de08a741f40c613ce894bb3234576b0e4774692cd32ec5b479472bf3b3e6`  
		Last Modified: Thu, 21 Jul 2022 02:33:14 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
