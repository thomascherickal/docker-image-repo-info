## `maven:3-openjdk-16`

```console
$ docker pull maven@sha256:5f02e9d85ae192057a30464110525a0dc4131b32c1a9ec26d8f588effc7ddd84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-16` - linux; amd64

```console
$ docker pull maven@sha256:0f2ae2653be5858fe91c3b65751dff4a3eb90e145f198acf2c4e69c74371cb5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.1 MB (397114516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9be56d735970cc2b90cdc4acb4d2778b6da80318d970953e7ce65828ee65d229`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 15 Sep 2020 21:22:07 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Fri, 30 Oct 2020 02:05:51 GMT
ADD file:ca74b6a4572ba9ecd7ceca8360a2d15560bf779277672ae9a37e25c53f8d1226 in / 
# Fri, 30 Oct 2020 02:05:51 GMT
CMD ["/bin/bash"]
# Fri, 30 Oct 2020 04:37:30 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 30 Oct 2020 04:37:30 GMT
ENV LANG=C.UTF-8
# Fri, 30 Oct 2020 04:37:30 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 30 Oct 2020 04:37:31 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 Nov 2020 23:30:16 GMT
ENV JAVA_VERSION=16-ea+22
# Mon, 02 Nov 2020 23:30:54 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/22/GPL/openjdk-16-ea+22_linux-aarch64_bin.tar.gz; 			downloadSha256=c206d6ea6855791a33ca7ff37363a53db4382ec0864d1662bc60f4dd0236a035; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/22/GPL/openjdk-16-ea+22_linux-x64_bin.tar.gz; 			downloadSha256=90b7e4e4945ca2d728ea2206739a0022aac50c47c3fb4078b8274ba7aab91c31; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 02 Nov 2020 23:30:54 GMT
CMD ["jshell"]
# Tue, 03 Nov 2020 00:01:07 GMT
ARG MAVEN_VERSION=3.6.3
# Tue, 03 Nov 2020 00:01:07 GMT
ARG USER_HOME_DIR=/root
# Tue, 03 Nov 2020 00:01:07 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Tue, 03 Nov 2020 00:01:08 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Wed, 04 Nov 2020 19:34:42 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN microdnf install findutils git
# Wed, 04 Nov 2020 19:34:46 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 04 Nov 2020 19:34:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 04 Nov 2020 19:34:46 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 04 Nov 2020 19:34:46 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 04 Nov 2020 19:34:47 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 04 Nov 2020 19:34:47 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 04 Nov 2020 19:34:47 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:9f8aeb516aa1b01143452930dec1cadef36b4298bcdb43224755b12ab4bc9289`  
		Last Modified: Fri, 30 Oct 2020 02:07:57 GMT  
		Size: 54.2 MB (54163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6199265ff0195874d7975d360d91e2ed48bc621c12633d52a4fe5207953ff202`  
		Last Modified: Fri, 30 Oct 2020 04:42:34 GMT  
		Size: 13.5 MB (13508533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b8536deb45e66bf2d2495bb7040c41ce5e2acd8cd0276eb9718b4ee22b6d78`  
		Last Modified: Mon, 02 Nov 2020 23:34:45 GMT  
		Size: 199.0 MB (199012893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49859e00b1f7d95049ce1edb5441deb2b7e521f5a00ae2cd150c461b1b5bd40`  
		Last Modified: Wed, 04 Nov 2020 19:38:29 GMT  
		Size: 120.8 MB (120847644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5165a906ed3a0f5adfe2b12a24a75fbd0df660a7c4a47963900b5d98fe791179`  
		Last Modified: Wed, 04 Nov 2020 19:38:18 GMT  
		Size: 9.6 MB (9581210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4138db13296b9e3a4dda14591beb6406ae0d5decac7e75500e53bc15455cb176`  
		Last Modified: Wed, 04 Nov 2020 19:38:17 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33f3533fe2cdfe81a9b560b50ba77bcdb98f9bb13c7943514b92e1ca36cfb76`  
		Last Modified: Wed, 04 Nov 2020 19:38:18 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-16` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:81a9f406b341d2457d68ee6fbed681daab9b22669a0bc9e74f7d12e44d1b22f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (352953712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b9be214d6cabe66f5aade04be15bf3503dd9634f2af489608d74b79cc16f81`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 15 Sep 2020 20:40:54 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Fri, 30 Oct 2020 03:44:45 GMT
ADD file:9cec0313dda06011e5a2f413448db8dc2a3f2e6305dbfd3afa2f78c9e571c080 in / 
# Fri, 30 Oct 2020 03:44:49 GMT
CMD ["/bin/bash"]
# Fri, 30 Oct 2020 04:03:41 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 30 Oct 2020 04:03:42 GMT
ENV LANG=C.UTF-8
# Fri, 30 Oct 2020 04:03:42 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 30 Oct 2020 04:03:43 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Nov 2020 00:24:25 GMT
ENV JAVA_VERSION=16-ea+22
# Tue, 03 Nov 2020 00:25:07 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/22/GPL/openjdk-16-ea+22_linux-aarch64_bin.tar.gz; 			downloadSha256=c206d6ea6855791a33ca7ff37363a53db4382ec0864d1662bc60f4dd0236a035; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/22/GPL/openjdk-16-ea+22_linux-x64_bin.tar.gz; 			downloadSha256=90b7e4e4945ca2d728ea2206739a0022aac50c47c3fb4078b8274ba7aab91c31; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 03 Nov 2020 00:25:08 GMT
CMD ["jshell"]
# Tue, 03 Nov 2020 01:05:18 GMT
ARG MAVEN_VERSION=3.6.3
# Tue, 03 Nov 2020 01:05:19 GMT
ARG USER_HOME_DIR=/root
# Tue, 03 Nov 2020 01:05:20 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Tue, 03 Nov 2020 01:05:20 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Wed, 04 Nov 2020 19:56:42 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN microdnf install findutils git
# Wed, 04 Nov 2020 19:56:53 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 04 Nov 2020 19:56:54 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 04 Nov 2020 19:56:55 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 04 Nov 2020 19:56:55 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 04 Nov 2020 19:56:56 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 04 Nov 2020 19:56:57 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 04 Nov 2020 19:56:57 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e3e30b00fc3497706dcd32508109092c83b0a5b47bd1dbd485dc8a0da352da68`  
		Last Modified: Fri, 30 Oct 2020 03:46:38 GMT  
		Size: 54.3 MB (54268366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2870a34311e6e2480637a34f3904b567d224baff73277563033ebcee672d93`  
		Last Modified: Fri, 30 Oct 2020 04:11:09 GMT  
		Size: 14.4 MB (14365455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f573ee8059a401f058fc459292bc3a7e34eac9453dae08c55827e2faa72abd`  
		Last Modified: Tue, 03 Nov 2020 00:31:51 GMT  
		Size: 177.6 MB (177563920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b9567d97aa28298466b8514ffed58445a2d398d1ae083e5e06e216665be3c4`  
		Last Modified: Wed, 04 Nov 2020 20:00:58 GMT  
		Size: 97.2 MB (97173553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea67120608386f25f7da5fa7f2b99b40990c5f618380db239a8cfea4a7157ad`  
		Last Modified: Wed, 04 Nov 2020 20:00:43 GMT  
		Size: 9.6 MB (9581200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc78b34f20aa94412565d185da67f82000b0e1a6d417092fd17b6eaf7fb3f0b`  
		Last Modified: Wed, 04 Nov 2020 20:00:41 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9344428c5b588a276e1c95ab882e14bf9380e0297a072bf499e9bbdb5474200`  
		Last Modified: Wed, 04 Nov 2020 20:00:41 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
