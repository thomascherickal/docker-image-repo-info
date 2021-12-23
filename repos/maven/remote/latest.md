## `maven:latest`

```console
$ docker pull maven@sha256:208ceab2ef5edc2845e18942fd63a153842ed7a098687321a8012c53c0b5b3ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:latest` - linux; amd64

```console
$ docker pull maven@sha256:b52dfe7b058e3db1cd677a0b1d0fa618f3b9e891d7cd1549f3c3d1c12aa6acbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.6 MB (424636997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59fcf607b5128e18da32a7c5c11cacdc53a36e08b66ab49c0cb4a50509bd7b91`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 23 Dec 2021 02:20:57 GMT
ADD file:15b307e0b1aafead42c103e34d3e51a271acea1ab0b68961e239f11af3b0d179 in / 
# Thu, 23 Dec 2021 02:20:57 GMT
CMD ["/bin/bash"]
# Thu, 23 Dec 2021 02:37:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Dec 2021 02:39:05 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Thu, 23 Dec 2021 02:39:05 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Dec 2021 02:39:05 GMT
ENV LANG=C.UTF-8
# Thu, 23 Dec 2021 02:39:05 GMT
ENV JAVA_VERSION=17.0.1
# Thu, 23 Dec 2021 02:39:16 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='1c0a73cbb863aad579b967316bf17673b8f98a9bb938602a140ba2e5c38f880a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='86653d48787e5a1c029df10da7808194fe8bd931ddd72ff3d42850bf1afb317e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 23 Dec 2021 02:39:16 GMT
CMD ["jshell"]
# Thu, 23 Dec 2021 03:44:11 GMT
ARG MAVEN_VERSION=3.8.4
# Thu, 23 Dec 2021 03:44:12 GMT
ARG USER_HOME_DIR=/root
# Thu, 23 Dec 2021 03:44:12 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Thu, 23 Dec 2021 03:44:12 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Thu, 23 Dec 2021 03:44:40 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN microdnf install findutils git
# Thu, 23 Dec 2021 03:44:43 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 23 Dec 2021 03:44:43 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 23 Dec 2021 03:44:43 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 23 Dec 2021 03:44:43 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 23 Dec 2021 03:44:43 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 23 Dec 2021 03:44:44 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 23 Dec 2021 03:44:44 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:155aced2666332ddff5a741b0236f360820e7aa3fc3dde2224fc17a91fc48db6`  
		Last Modified: Thu, 23 Dec 2021 02:21:56 GMT  
		Size: 42.1 MB (42105152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5901c58ecb29b61159b5e3a63dfbb0fb520b2de1d33c9fb038d9b697e3fcd4`  
		Last Modified: Thu, 23 Dec 2021 02:45:32 GMT  
		Size: 13.5 MB (13520734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1076e441ffb58eee60f1bab40db6ca69a01e33346eff212eac1191e6b754bd`  
		Last Modified: Thu, 23 Dec 2021 02:47:53 GMT  
		Size: 187.2 MB (187170395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ebe02efffc96452268587edf1aaf04a0579ef682b6d2b58130276c45cd54d0`  
		Last Modified: Thu, 23 Dec 2021 03:46:56 GMT  
		Size: 172.7 MB (172729692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bdcfcd579d036e52ad15d5a3a1f6432a345b5f34255558d36b70fd92a3c191`  
		Last Modified: Thu, 23 Dec 2021 03:46:43 GMT  
		Size: 9.1 MB (9109811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5c4a9531a45594e3f9e1a10bba4a4dadd5a94ee779d55514d9894d950d301c`  
		Last Modified: Thu, 23 Dec 2021 03:46:42 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d31dfa25635e71ab0b281b894c6e444c65cb7dd29e2d87121b28f3372ec8e57`  
		Last Modified: Thu, 23 Dec 2021 03:46:42 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:latest` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:d0afae46fb2c1448d5b2b8b5195077ff3321933e03d5afc8619cbf72e964969d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.1 MB (412092416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9940efec717d8ad8c4a160c8b55a4c13bc9859042fe05d9bdf7390f8d70c565`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 23 Dec 2021 02:40:45 GMT
ADD file:140d632303428d802f77f473aef33fa52daacdfc76b23edde4344be661c1d4b0 in / 
# Thu, 23 Dec 2021 02:40:46 GMT
CMD ["/bin/bash"]
# Thu, 23 Dec 2021 02:58:38 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Dec 2021 02:59:40 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Thu, 23 Dec 2021 02:59:41 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Dec 2021 02:59:42 GMT
ENV LANG=C.UTF-8
# Thu, 23 Dec 2021 02:59:43 GMT
ENV JAVA_VERSION=17.0.1
# Thu, 23 Dec 2021 02:59:54 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='1c0a73cbb863aad579b967316bf17673b8f98a9bb938602a140ba2e5c38f880a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='86653d48787e5a1c029df10da7808194fe8bd931ddd72ff3d42850bf1afb317e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 23 Dec 2021 02:59:54 GMT
CMD ["jshell"]
# Thu, 23 Dec 2021 03:51:58 GMT
ARG MAVEN_VERSION=3.8.4
# Thu, 23 Dec 2021 03:51:59 GMT
ARG USER_HOME_DIR=/root
# Thu, 23 Dec 2021 03:52:00 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Thu, 23 Dec 2021 03:52:01 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Thu, 23 Dec 2021 03:52:36 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN microdnf install findutils git
# Thu, 23 Dec 2021 03:52:47 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 23 Dec 2021 03:52:48 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 23 Dec 2021 03:52:49 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 23 Dec 2021 03:52:51 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 23 Dec 2021 03:52:52 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 23 Dec 2021 03:52:52 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 23 Dec 2021 03:52:53 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:53f096d4aa0757c30613f325df1e03a90db9d9879ea251b394e3ab0a068b5610`  
		Last Modified: Thu, 23 Dec 2021 02:41:44 GMT  
		Size: 42.0 MB (42018351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921862a08fd8bc652539d62804daf06ab6464bd5b42061f5bedbdfa73bd62136`  
		Last Modified: Thu, 23 Dec 2021 03:11:46 GMT  
		Size: 14.3 MB (14303905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e5e67fcac32d1d4b20751372e66e4b457cc5644d14505043285d47f485d041`  
		Last Modified: Thu, 23 Dec 2021 03:13:18 GMT  
		Size: 186.0 MB (185976992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14e3f35d4fd76fd23b590cca800b43e9d6cc38d74e66afd5e509126c786e3f8`  
		Last Modified: Thu, 23 Dec 2021 03:56:08 GMT  
		Size: 160.7 MB (160682174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35761e43f9a71333e20708dbc224cc6432542939789e2e2e5c36e2e18ea4466`  
		Last Modified: Thu, 23 Dec 2021 03:55:53 GMT  
		Size: 9.1 MB (9109775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdbcac22c631328a424c094dd7f0d4d11a7885dad423f410e8eaf48a52ed8de`  
		Last Modified: Thu, 23 Dec 2021 03:55:52 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e08c68dc89b59dc0a91ad5e0cb7c773bc159c7c47f5dadf90be33eb7a60c6f`  
		Last Modified: Thu, 23 Dec 2021 03:55:52 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
